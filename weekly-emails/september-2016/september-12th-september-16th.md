## Microstates

[Microstates][1] is a library for expressing "pure" reusable state
machines. Each state is immutable, transition is a function with no
side-effects.

This week, Taras, the Ember Sherpa and I will be pairing to lay the
groundwork for the basic state machines. These are state machines
describing things like a boolean value, a number value, list value,
etc... If you're interested in helping out, these should be very
digestible and lot's of fun! You can track development in the
[microstates channel in the Ember community slack][2].

[1]: https://github.com/cowboyd/microstates.js
[2]: https://embercommunity.slack.com/messages/e-microstates

## Mocha Snippets

[Mocha snippets][3] are a set of handly templates for generating mocha code
when you're writing mocha tests. It let's you do things like type
`desc` and it will drop:

``` javascript
describe('something', function() {

});
```

Into your buffer.

The only problem is that some folks don't want
`'something'` They like `"something"`. Yet other folks still dislike
using the "classic" `function` syntax and prefer ES6.

I had a few extra hours this weekend, so I decided to make these
templates customizable, so now you can make it go:

``` javascript
describe("something", ()= {

});
```

If that's what you want.

It was a fun break from JavaScript. Snippets are one of my favorite
editor features, and one that is _such_ a timesaver. In fact, I think
it's just a great topic that I'll be giving a lunch on basic
snippeting in emacs this Friday.

[3]: https://github.com/cowboyd/mocha-snippets.el
