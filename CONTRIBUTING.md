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
