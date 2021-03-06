# What is oss-wumbo?

oss-wumbo is a public repo The Frontside uses to interface with the
community at a meta level. The purpose of this repo is for you to gain a
deeper understanding of what open source projects we're currently
working on at The Frontside and where those projects are heading.

Our goal is to be working openly and documenting our direction if it
pertains to open source. This is so the users of our software can have
insight into what is next for the project they're relying on. We're
always looking for ways to improve how we collaborate with the
community. If the users want to, they can provide feedback and have
an impact on our process or projects. This repo is open source, so you can
[open an issue!](https://github.com/thefrontside/oss-wumbo/issues/new)

## Why is OSS important to The Frontside?

We take open source pretty seriously at the Frontside because we
strongly believe in giving back to the programming community. As a
consultancy, we see many of the same problems in client apps crop up
again, and again, and again, and this is how most of our open source
projects are born.

By actively identifying shared problems, we are able to develop shared
solutions solutions, and by open sourcing these solutions we allow
their consumers to report bugs and contribute back. This creates a
much stronger piece of software which is great for **everyone
involved**. That means you, our clients, and the community at large.

Lastly, owning code is very expensive. This is because if
you own a project, you have to manage that project and make sure your users
are happy. We're more than willing to take the responsibility that our
open source projects avoids the dreaded
[bit rot](http://www.catb.org/jargon/html/B/bit-rot.html) so that our
community can experience the benefits of code ownership without having
to continually shoulder its costs.

## What is a project champion?

A project champion is a person who is the main manager of an open
source repo. We need project champions because unowned projects tend
to rot. If someone "owns" a repo, they're responsible for making sure
that repos community is healthy. This person will have the most
context of the project and documents the road map of the project. **This
does not mean they do all the work.**

Some of the responsibilities for being a project champion are:

- Keeping the project up to date
  - Managing dependencies
  - Not letting PRs get stale
  - Not letting issues get stale or unanswered
- Managing & replying to issues
  - Add proper labels
  - Add proper release milestones
- Assigning PRs for review
- Setting release milestones
- Publishing the road map
- **Delegating tasks when needed**

Being a project champion means managing the code is only half of the
battle. You're managing a small community that uses your project.
You also fill a support role for people who need help using the
project. It's very important to foster this community! You can find
the list of projects and [their champions here](http://github.com/thefrontside/oss-wumbo/project-champions.md).

## What should a Frontside OS repo include?

Our goal is to provide the best OS software to the community. This
means each one of our addons must fill a gap in the ecosystem, not
reinvent things. Owning code is expensive after all. For us to declare
an OS repo to be in good standing condition it must include the
following:

  - Contributing.md
    - How to build the source code
    - How to run the tests
    - The best way to get your PR accepted
  - Issue template
  - PR template
  - Changelog.md
  - Code Of Conduct
  - Fully filled out package.json
  - Fully filled out "Description" & "Website" inputs on GitHub
  - Organize releases with milestones
  - Nicely designed, uniformly branded example pages
  - Cross browser test all the things
  - Auto publishing `gh-pages` from CI
  - Organized issues with labels (standardized labels)
    - Bug
    - Won't fix
    - Documentation
    - Feature
    - Good for beginners
    - Investigate
    - Waiting for response
    - Dependency update
  - A filled out README with the following:
    - badges
      - released version
      - version compatibility
      - build status
    - Describe what problem does this solve for me?
    - Show exactly how you would use this in an app
    - Link to a demonstration in action
    - Section for those who are *Stuck*
      - tweet
      - pairing hours
      - Contributors are visible, and easy to reach
