Hey everyone! We've got a couple weeks of OSS to catch up on.

First I'd like to say the first phase of the `oss-weekly-mailer` rails
app has been completed! Now when you merge a PR on the `oss-wumbo`
repo with a title `Weekly email:` it will scoop up that markdown file
& email it to our project updates list. That means I'm not the only
one that can write these emails! ;)

I'm also going to switch up the format a little to experiment. Let me
know your thoughts!


### Charles

I’m happy to report that I was able to grab 2 hours on friday to make
some real progress on microstates, and I couldn’t be happier with the
result. I’ve been working on the low-low level microstate library
which, if anybody asks you what it is, is a JavaScript DSL for
expressing immutable state machines.

I was able to rewrite the core state primitive to dogfood its own
transitions, and I think I have a really simple solution for handling
nested states. If I can tackle that this week, then it might be ready
to start bringing it a level up the stack: embedding them into ember
or embedding them into
observables. [Checkout the PR here.](https://github.com/cowboyd/microstates.js/pull/13)

There was a lot of *exciting* movement on the `ember-let` front over
the weekend too. I had merged a pull request from Taras that allowed
you to use the `{{let}}` helper in inline form. While this
demonstrated the style, the actual variable binding semantics were
“not that great” :tm:

Luckily, open source heroes Robert Jackson and Martin Muñoz swooped in
and re-implemented it as a handlebars syntax transform, so that now we
have true (almost) `let` semantics in the JavaScript and Lisp sense of
the
word. [Check it out here!](https://github.com/thefrontside/ember-let/pull/12)

### Stephanie

Worked some more on the acceptance test for the learning app. Created
the model hook, I commented out the original array and stubbed it with
mirage but that’s as far as I got because I was getting a weird 404
error. I posted my code in the ember slack, mirage channel on Friday
if you want to take a look- there’s been no replies. My goal is to get
unstuck with mirage & finish the acceptance test.

### Robert

Over the past two weeks I've worked on our new website and getting the
styling in place. I'm currently in the middle of styling the blog show
page. I do have a question or two regarding the large header but that
can be address in our weekly website meeting. Hopefully this can be
wrapped up nicely by the end of the week.

I also attempted to cut a release for `emberx-file-input` but ran into
some CI failures for Ember 1.13 over a dependency I think. Locally I
cannot reproduce which makes this interesting to debug. I'm going to
have to figure out what's going on with that this week and cut a new
release.

Lastly I was able to wrap up the first part of the `oss-weekly-mailer`
app. Right now it will shoot off an email once a PR is merged with
`Weekly email:` in the title. It's now tested and pushed up to heroku
waiting for your PR events. Next steps for this app is to start
pulling and storing metrics of our OSS to send along with each
email. That's going to be fun!
