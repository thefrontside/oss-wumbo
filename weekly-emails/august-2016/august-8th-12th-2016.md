Good morning everyone! I'm a little late on sending this OSS weekly
out :( The awesome thing is, this is the first time we've missed since
starting this over a month ago!

Alex worked on Impagination last week but did not get any closer
to his goal of 90% test suite passing. He mainly worked on an Observer
class which allows for better testing and is a model for how
Ember-Impagination will consume Impagination.

This week Alex is going to do a little change up and work on the
frontside website instead of imapgination. He made progress on the
website and opened a [Middleman - Ember Islands spike](https://github.com/flexyford/middleman-project-v4/pull/1) on his personal
repository. His goal is to get Ember-Islands running in Middlemans External
Pipeline (which replaces the Rails Asset Pipeline).

Stephanie worked with Brandon last week was able to come up with a breakdown
of what they think will be the ‘app’ portion of the website. They also
started an ember app called `partyfavors` - it’s literally nothing
more than `ember new` since they didn’t get far on a Friday Interview
day. There were some issues like both middleman and ember want to
observe and there’s another issue with sprockets.

She's not sure what to tackle next on her OS day this week because
she's kind of stuck. If anyone sees anything they want to pick off the trello-
please leave a comment on trello or GH so that everyone else knows.

Charles did not make any progress on microstates or on his blogpost.
Which is bad because there are people asking about it! :p It’s also
running the risk of becoming perpetual vaporware.

What he wants to do this week is to maybe setup a hangout mostly for
Chris and Charles, but also for anybody else interested to talk about
things and try and document and  thereby enable the work that needs to
be done to be done in parallel. _(Rob note: Try documenting this
publically within the repo so anyone can contribute if they
want. Leverage community!)_

Brandon did open a [PR on x-select](https://github.com/thefrontside/emberx-select/pull/135) fixing a bug where the default value
wasn't being fired off the first time if you're using the `one-way`
flag. This week he's enjoying the goregous Flordia beaches on
vaction.

For me I'm finally going to ship the "what is oss-wumbo" branch I've
had going for far too long. I also did a lot of work to the
emberx-file-input repo. Cleaned up some import fires that happened &
worked with Jeffery in his interview to [add a way to reset the input](https://github.com/thefrontside/emberx-file-input/pull/37)
once the action has fired so you can select the same file multiple
times. There was also some work done to add a [default `alt` attribute](https://github.com/thefrontside/emberx-file-input/pull/39)
for the blockless version of x-file-input.

This week I'd like to cut version 1.1.0 of x-file-input and get
rolling on v3.0 of x-select. I'd like to have at least one v3.0 tagged
issue closed for x-select.

I hope everyone has a great week! :)
