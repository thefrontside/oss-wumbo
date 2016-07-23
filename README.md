# What is oss-wumbo?

oss-wumbo is a public repo The Frontside uses to interface with the
public at a meta level. The purpose of this repo is for you to gain a
deeper understanding of what open source projects we're currently
working on at The Frontside and where those projects are heading.

Our goal is if it pertains to open source we should be working in the
open and documenting our direction. This is so the users of our
software can have insight into what is next for the project they're
relying on. We're always looking for ways to improve how we
collaborate with the community.  If the users want to, they can
provide feedback and have an impact on our process or projects. This
repo is open source, so you can
[open an issue!](https://github.com/thefrontside/oss-wumbo/issues/new)

## Why is OSS important to The Frontside?

TODO

## What is a project champion?

A project champion is a person who is the main manager of an open
source repo. We need project champions because unowned projects tend
to rot. If somone "owns" a repo, they're repsonsible for making sure
that repos community is healthy. This person will have the most
context of the project and documents the roadmap of the project. **This
does not mean they do all the work.**

Some of the responsibilities for being a project champion are:

- Keeping the project up to date
  - Managing dependecies
  - Not letting PRs get stale
  - Not letting issues get stale or unanswered
- Managing & replying to issues
  - Add proper labels
  - Add proper release milestones
- Assigning PRs for review
- Setting release milestones
- Publishing the roadmap
- **Delegating tasks when needed**

Being a project champion means managing the code is only half of the
battle. You're managing a small community that uses your project with
it. You also fill a support role for people who need help using the
project. It's very important to foster this community! You can find
the list of projects and [their champions here](http://github.com/thefrontside/oss-wumbo/project-champions.md).

## What should a Frontside OS repo include?

Our goal is to provide the best OS software to the community. This
means each one of our addons must fill an a gap in the ecosystem, not
reivent things. Owning code is expensive after all. For us to declare
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
    - Dependecy update
  - A filled out readme with the following:
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
