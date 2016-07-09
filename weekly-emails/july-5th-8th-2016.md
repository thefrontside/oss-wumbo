Hey everyone! This is the first week of our new OSS process. I'm
really happy with the new direction we're taking and I think it's
going to show when we start shipping regularly. That's the name of the
game here. We want to ship quality and well maintained open source
software. Exciting times!

For these weekly emails they should be fairly quick and to the
point. Whoever is writing the email can add any kind of flavor they
please, so have fun with it!

The email should include a couple key things:

- Who is doing what
- What do they expect to get done this week
- Any quick updates for projects
- Who's blocked on what (like a call to unstick this person)

For this week:

Alex, Stephanie, and I have set goals to make progress on our
respective projects we champion.

Alex is working on impagination proper, and is trying to figure out
the right API for the pages interface. He expects it to be lazily
loaded (like the records interface is currently) for performance
reasons. This week his goal is to finalize the pages interface API &
TDD that API.

Stephanie is working on the new Frontside website and has been stuck
for the past two weeks porting the old blogs over to the new middleman
site. Her goal for this week is complete the migration. Brandon
offered to help but if he can’t we should make sure we get her
unblocked. The website has a target launch date of August 1st and is
important to the business, so we should make it a priority.

I’m going to be working on, you guessed it, emberx-select! My goal for
the week is ship v2.2.0 of x-select that includes the option to turn
off two-way data binding. This will set the stage for v3.0.0 because
we’re turning off two-way data binding by default. This change might
require a refactor with how we test. I’d like to have an offline
discussion about whether it’s a good idea to build an application in
our dummy apps as a test bed. I’ve discovered it requires some
maintenance when making changes.

Lastly, you can find this email in our new
[oss-wumbo](https://github.com/thefrontside/oss-wumbo) repo that will
be our interface to the public! It will house all of our OSS meta issues,
how we work, who is a project champion of what, what that even means,
each one of these emails, and many more things regarding OSS at The
Frontside.

Okay, that’s enough for now. I’m excited to start shippin’ some code
with y’all! LETS GET IT!
