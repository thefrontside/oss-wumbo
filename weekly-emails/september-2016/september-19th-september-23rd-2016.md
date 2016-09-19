## x-select

There was a flurry of activity on x-select last week! Stanley & the
Heroku crew seem to be updating their ember app which made them
discover some bugs with x-select & they were nice enough to help patch
those bugs by submitting some really awesome PRs:

- Coalesce registering and unregistering options ([#147](https://github.com/thefrontside/emberx-select/pull/147))
- Call willDestroyElement's `this._super` last ([#148](https://github.com/thefrontside/emberx-select/pull/148))
- Reduce number of components searched ([#149](https://github.com/thefrontside/emberx-select/pull/149))
- Don't share `options` arrays between x-select instances ([#150](https://github.com/thefrontside/emberx-select/pull/150))
- Fix bug where undefined initial values were changed to null ([#152](https://github.com/thefrontside/emberx-select/pull/152))
- Guard against `__setDefaultValues` being called during teardown ([#153](https://github.com/thefrontside/emberx-select/pull/153))

And those are just the PRs they submitted! I was also able to land
firing an action when an option becomes disabled
([#146](https://github.com/thefrontside/emberx-select/pull/146)) &
auto deploying on CI success
([#154](https://github.com/thefrontside/emberx-select/pull/154)). If
that doesn't show the power of community to you, I don't know what
will :P

Currently in the works is moving all of the tests into a `test-bed`
route & styling our demo page to look nice & clean. What should fall
out of that is a "Frontside branding" ember addon for us to pull into
all our other addons.


## website

The `search-filter` component now successfully returns the relevant cards when a
user types a query in the search input box.

Next step is to refactor the search box and its actions so that the box resides
inside the nav bar. Then I will create the parent component `media-filter` and
update the tests.

We now have a fully responsive layout for the site's header/footer and the homepage.
Next steps: start subpages, finish content piece component, create blog index, photo grid on homepage

## emberx-form

Last week was the first full day that's been committed to x-form-related OSS work! Since x-form has been put to use, we've discovered a number of pain points (a.k.a. "opportunities for improvement") regarding its usage of `ember-changeset` and how it handles deeply nested object.

To that end, I've started working on library that tries to build up the "buffer"-like behavior in a way that is immutable and not at all Ember-specific. It's currently called [change-buffer](https://github.com/cafreeman/change-buffer). I did some work last week on getting it into a usable format (it's technically on npm now!).  In addition, I did a spike on consuming `change-buffer` in `x-form`, with mixed results.

This week, I'll be working on how to best handle the issue of rollbacks in `change-buffer` in a way that actually works in Ember. Currently, the rollback works fine with regard to the actual data, but Ember doesn't update the DOM :(.
