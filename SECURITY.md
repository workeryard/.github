# Security

Please report a vulnerability privately, not in a public issue: open the
repository's **Security** tab and choose **Report a vulnerability**. You will
hear back within a week.

A repository with a `SECURITY.md` of its own says there what counts for it.
Where it does not, a vulnerability is anything that lets an attacker:

- read or alter data a caller did not hand them;
- make a library accept what it is meant to refuse;
- make a Worker do work the attacker chose.

Fixes go into the latest release of the library. Older releases are not
patched.
