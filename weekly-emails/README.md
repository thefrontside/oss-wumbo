# What is the weekly email?

At the Frontside we meet for 15 mins each monday and discuss what we
were able to accomplish last week with our open source effort and what
our goals are for the up coming week. These are published openly here
in our oss-wumbo repo and then also sent to everyone who works at the
Frontside.

## How do I run the meeting?

The meeting should be time boxed to 15 minutes. It's very important to keep
these meetings short and sweet so they're not taking away too much
time for client projects. It should be a hard stop at 15 minutes.

The basic format of the meeting is to go around the room and ask each
person:

  - What they worked on last week
  - Were there any wins?
  - Are you stuck?
  - Anything exciting to share?
  - What their goal for this week is

## What should go into the email?

The weekly emails should be fairly quick and to the point. Whoever is
writing the email can add any kind of flavor they please, so have fun with it!

The email should include a couple key things:

  - What they were able to accomplish last week (think of it like
celebrating wins!)
  - Who is working on what project & what task
  - Any quick updates for projects
  - Who's blocked on what (like a call to unstick this person)
  - What do they expect to get done this week

You can find the template for the weekly
[oss meeting here](http://github.com/thefrontside/oss-wumbo/weekly-emails/meeting-template.md).


## How to send the email

Once you've complied all the notes you need to send the email, open a
PR and add the `weekly email` label and send it out for review. It's
very important for you to add the `weekly email` label to the PR or
else it will never be sent out as an email. 90% of the time you don't
need to wait for anyone to review your PR.

Once you merge the PR magic will happen. This is why the label is
important. We have a [rails app](TODO) that scoops up the markdown,
parses it, adds some nice little stats, and sends it off in a nicely
formatted email.
