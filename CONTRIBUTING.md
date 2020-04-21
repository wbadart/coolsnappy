# Contributing

Thank you for your interest in contributing to coolsnappy!

coolsnappy is a very early-phase project; we're still scoping out the design,
and haven't even written any code yet. This makes contributing a little
abnormal compared to other open source projects, which readily accept bug
reports, feature requests, and the like. We'll get there in due time.

In the meantime, there are two ways to help the project out:

1. Participate in design discussions
1. Contribute documentation

## Design Discussions

Public discussions take place primarily on [open issues][02], especially issues
belonging to the [active sprint][03]. We welcome your thoughts, questions, and
ideas, which you may share as a comment on any thread.

We also welcome and appreciate comments not aligned to an existing ticket. You
can share these by opening a new issue. **Please align your issue to the
_Backlog_ project, where it can be triaged.** When you create your issue,
you'll see the template for a user story. We use this almost exclusively during
sprint planning meetings (more on that in a moment) so in the likely case this
doesn't fit your discussion, open a [blank issue][04] instead.

In addition to the rolling conversations that happen in the issue tracker,
there is a biweekly sprint planning session which takes place on the
`#coolsnappy` channel of [functionalprogramming.slack.com][01]. In general,
this will be every other Monday starting April 13 2020. See the channel for
further schedule details and updates. The purpose of this meeting is to review
recent progress and decide what work needs to be done in the project's
immediate future (the next two weeks). Contributions will be welcome on any
part of the project at any time, though in general the maintainers will be
focused on (and therefore prioritize) work discussed at the prior planning
session.

## Documentation Contributions

Despite being a little code-light at this phase, we still have some
documentation, which will be updated lots in the coming weeks. If something in
the documentation doesn't align with the current design and goals of the
project, we welcome pull requests!

> **Working on your first Pull Request?** You can learn how from this
> **free** series [How to Contribute to an Open Source Project on
> GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github)

For the sake of consistency, markdown files should adhere to the [default
rules][07] of the `mdl` markdown linter. There's a GitHub [Action][06] which
will run the check for you, but you can also run the check locally with docker
(from the project root):

```sh
docker run --rm -v $PWD:/src:ro rsrchboy/mdl /src
```

Or directly with ruby:

```sh
gem install mdl && mdl .
```

### Creating a PR

There are a couple items we'd like you to keep in mind as you craft your PR
that will help us review your changes and get your contribution merged as fast
as possible.

#### Atomic, Readable Diffs

Every PR will need to be reviewed before it's merged (even those from
maintainers). PRs, therefore, should be optimized for the review process.

There might be lots you want to contribute, but it's easiest to review change
sets one at a time. Focus your PR on a single contribution. Look at the diff
from the perspective of a reviewer and ask yourself, does every little bit of
red and green relate to the one problem I'm trying to solve? This will be
easier if the commits which comprise your PR are themselves [atomic][08].

You can open a PR that isn't quite ready for review as a [draft][09]. This is a
great way to get early feedback and discussion about an idea, even before the
"formal" review process begins.

#### Closing Keywords

[Closing keywords][10] are a fantastic feature of GitHub that play marvelously
with project board automation. If your PR will fully address an issue, we
encourage you to link that issue using the special syntax. **However**, if the
issue has explicitly listed its acceptance criteria, we ask that you copy those
bullet points into a blockquote in the body of your PR and explain (if briefly)
how the proposed changes address each requirement. See [#6][11] for an example.

#### Status Checks

Please address any failed status checks on your PR before requesting review. We
won't be able to merge it until it passes anyway.

#### Metadata

GitHub gives you the option (in the menu on the right-hand side of the PR
creation page) to attach all manner of metadata to your issue. You can mostly
leave these alone, other than adding an appropriate label if you see fit. This
will most likely be one of `documentation`, `bug`, or `enhancement`. (Sizes and
story/ task/ epic are reserved for issues.)

The assignee is the person responsible for seeing the PR through to completion.
This is mostly you, with a little bit from the maintainer who clicks the
"merge" button at the end of the process. Single-commit PRs can be rebased and
merged, while all others should create a merge commit (the default option). The
working branch should be based on the current `master` commit to support a
pseudo-linear history (all commits are sequential, other than merge commits
which delineate work done).

A reviewer, by contrast, is only responsible for submitting feedback and either
requesting changes or approving the PR. In general, avoid submitting a review
for a draft PR.

---

coolsnappy is maintained by volunteers. We only have a few hours a week to
dedicate to the project, so we greatly appreciate your patience. And thank you
again for your interest in contributing. We look forward to welcoming you to
the coolsnappy community!

[01]: https://functionalprogramming.slack.com
[02]: https://github.com/wbadart/coolsnappy/issues
[03]: https://github.com/wbadart/coolsnappy/projects
[04]: https://github.com/wbadart/coolsnappy/issues/new
[06]: https://github.com/wbadart/coolsnappy/actions
[07]: https://github.com/markdownlint/markdownlint/blob/master/docs/RULES.md
[08]: https://curiousprogrammer.io/blog/how-to-craft-your-changes-into-small-atomic-commits-using-git
[09]: https://github.blog/2019-02-14-introducing-draft-pull-requests
[10]: https://help.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword
[11]: https://github.com/wbadart/coolsnappy/pull/6
