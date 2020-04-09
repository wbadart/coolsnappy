# coolsnappy

The survey framework that's too cool for school

Project coolsnappy aims to be a minimal, modular, and maintainable
tool for constructing survey systems.

**Minimal:** coolsnappy won't try to be more than it needs to be. It
starts with a core domain model of "surveys" and exports a small but
useful collection of functions for manipulating that domain.

**Modular:** coolsnappy won't be overly prescriptive about the parts
of the system you've already got covered. For example, we might ship
coolsnappy with a default storage backend (e.g. `sqlite`) but if you
bring your own database, coolsnappy should happily interface with
that instead.

**Maintainable:** you shouldn't need a PhD to pick up a coolsnappy
code base. We recognize that projects can change hands and we aim to
make that transition as smooth as possible by making code-grokking
the easiest part.

It might seem at this point that the primary goal of coolsnappy is to
make it easy to stand up survey systems. This is not the case.
coolsnappy's _primary_ goal is to explore technologies just outside
the mainstream to find interesting solutions for the above subgoals;
contributing to coolsnappy should be an educational experience.
