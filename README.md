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
strongly believe in giving back to the programming communities. As a
consultancy, we see many different problems in client
apps. Oftentimes, our OS projects are born out of solving a problem
for a client. We feel that we should be open sourcing our solutions
and giving back to the community.

We also strongly believe in community supported solutions. By open
sourcing software we allow consumers of the addons to report bugs and
contribute back to the project they are using. This creates a much
stronger addon which is great for **everyone involved**. That means
you, our clients, and the community at large.

Lastly, owning code is actually quite expensive. This is because if
you own it, you have to manage the project and make sure your users
are happy. We're more than willing to take the responsibility that
each and every one of our supported addons avoid the dreaded project rot.

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
battle. You're managing a small community that uses your project with
it. You also fill a support role for people who need help using the
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
