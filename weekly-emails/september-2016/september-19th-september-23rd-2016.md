## x-select

There was a flurry of activity on x-select last week! Stanley & the
Heroku crew seem to be updating their ember app which made them
discover some bugs with x-select & they were nice enough to help patch
those bugs by submitting some really awesome PRs:

- Coalesce registering and unregistering options ([#147](https://github.com/thefrontside/emberx-select/pull/147))
- Call willDestroyElement's this._super last ([#148](https://github.com/thefrontside/emberx-select/pull/148))
- Reduce number of components searched ([#149](https://github.com/thefrontside/emberx-select/pull/149))
- Don't share `options` arrays between x-select instances ([#150](https://github.com/thefrontside/emberx-select/pull/150))
- Fix bug where undefined initial values were changed to null ([#152](https://github.com/thefrontside/emberx-select/pull/152))
- Guard against __setDefaultValues being called during teardown ([#153](https://github.com/thefrontside/emberx-select/pull/153))

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
