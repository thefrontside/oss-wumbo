## x-select

Not a lot happened last week for x-select, but what we did start our
`fs-branding` addon that will hold all of our shared styles for OS
addons. You can find
[that addon here](https://github.com/thefrontside/fs-branding). It's
very much a WIP right now.

With x-select there's a branch right now that consumes that addon to
provide styling to our x-select dummy app. This week I hope to wrap
that up and get started on rewriting the readme to reflect what
x-selects goal is today.

## Website

The `media-filter` component was refactored so that now it is an
application and not a component like we originally planned.

The learning component was removed and everything was moved to application.
The `new-search` component handles searching and `search-filter` component
handles filtering the cards by media type. Now search operates on the same
level as fitlering by type.

Next step is to finish the acceptance and integration tests before passing
it on to be implemented on the learning page of the website.

## Microstates

Microstates is a tiny JavaScript library for expressing immutable
state machines. Part of what makes it special is the ability to
compose smaller state machines into larger state machines. An example
of a small state machine is one that wraps a boolean value:

```js
let bool = new Bool(true);
bool.toggle() //=> false
bool.toggle().toggle() //=> true
bool.set(false) //=> false
```

That's great, but in order to build bigger state machines, you need to
be able to embed smaller ones into the bigger ones. It does this by
mapping state transitions on the embedded states into state
transitions for the _entire state tree_.

Notice how if I toggle the left switch, I actually get a completely
new switchboard.

```js
let switchboard = new State({
  left: new Bool(false),
  right: new Bool(false)
})

switchboard.left.toggle() //=> {left: true, right: false }
```

This functionality was put in place last week, which leaves only two
more pieces in the puzzle before we can roll forward with it. The
first is allowing the containing state machine to "override" and/or
add transitions to the states that it contains. For example, let's say
that I want the left switch to operate indepedently, but I want the
right switch to always move in unison with the left. I.e. if I turn
the right switch on, I turn the left switch on too. If I turn it off,
then the left one moves. The left, however, does not affect the value
of the right.

```js
const Switchboard = State.extend({
  left: new Bool(false),
  right: new Bool(false),
  transitions: {
    right: {
      //override the right toggle action to toggle in unison.
      toggle(currentBoard, currentRight) {
        let newValue = !currentRight;
        return {left: newValue, right: newValue };
      }
    }
  }
});

let switchboard = new Switchboard();
switchboard.left.toggle() //=> { left: true, right: false }
switchboard.right.toggle() //=> { left: true, right: true }
```

I plan to put this in place this week, and then _*finally*_, it's off to
integrate with Ember, Redux and the planet!
