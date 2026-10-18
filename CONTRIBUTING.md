# Contributing

Issues and pull requests are welcome. A few things make them easier to take:

- **Show how you checked.** A change to what goes on the wire comes with what
  it was measured against — a capture, a server, a test — and the result
  before and after.
- **Run the checks.** Each repository says how; usually `make check`, and for
  code that runs in a Worker, `make typecheck-workers` too.
- **Keep it small.** One change per pull request, with tests. A new
  dependency needs a reason and a measurement of what it adds to a bundle.
- **Write it in English**, code and comments and commits alike. A commit says
  in its subject what it does, imperatively, and in its body why.

If a change is large, open an issue first, so the shape can be agreed before
the work is done.
