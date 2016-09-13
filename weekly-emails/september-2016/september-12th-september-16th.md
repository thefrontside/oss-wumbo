## Microstates

[Microstates][1] is a library for expressing "pure" reusable state
machines. Each state is immutable. Each transition is a function with no
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
using the "classic" `function` syntax and prefer ES6 fat arrows `()=>`.

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

## x-select

x-select 3.0 is pretty much feature complete at this point! 🎉 It now
only uses contextual components
([#140](https://github.com/thefrontside/emberx-select/issues/140)),
exports the select function
for use in integration tests (and more!)
([#141](https://github.com/thefrontside/emberx-select/issues/141)),
and two way data
binding is 100% dead
([#139](https://github.com/thefrontside/emberx-select/pull/139))!

The only things that are left before we ship 3.0 is moving the tests
off into their own test bed route
([#123](https://github.com/thefrontside/emberx-select/issues/123)) and
figuring out a way to deploy to
gh-pages (or maybe elsewhere?) after a successful master CI build
([#89](https://github.com/thefrontside/emberx-select/issues/89)).

I would like to get wrap those things up this week. When moving the
tests to their own route I want to have a new nicely designed demo
page for x-select -- which should be the standard for all our OSS
repos going forward.

## website


The learning page of the new website will have a component that will load
all the available learning resources like podcasts, blogs, and talks in the
form of cards. I've created a `media-filter` component that will render
these resource cards.

Last week I wrapped up the acceptance tests (for now), installed
`ember-bootstrap` and finished the filtering by resource type
functionality. These filter actions are linked to the podcast,
blog, and talk buttons that sit above the cards.

Next week I'd like to complete the search functionality so that
when a user types a query in the search input next to the buttons,
the cards will update asynchronously. So far I have created a `search-filter`
component and am working on making sure the tests are relevant and passing.
