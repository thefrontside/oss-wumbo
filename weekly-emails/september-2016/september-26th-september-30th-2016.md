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
