# WorkerYard

Open-source libraries for Cloudflare Workers.

## Who it is for

Developers building on Cloudflare Workers who reach the edge of what the
platform gives them, and need the missing piece done properly rather than done
again, by hand, in every project.

## Why

A Worker's built-in APIs are deliberately small. What they leave out tends to
be written once per project and checked against nothing. Each library here
takes one such gap and fills it well enough to depend on: small enough to
read, tested without the network, and checked against the real thing before a
release.

## How

- **Measured, not assumed.** A claim about the platform, a protocol or another
  system comes with how it was checked, and the check runs again before a
  release.
- **Reasons written down.** What was taken from other projects, what was left
  out, and why, lives in each repository's `docs/decisions.md`.
- **The runtime at arm's length.** A library's core takes what it needs from
  the runtime as arguments; the Workers adapter is one folder, so the rest
  runs and is tested anywhere.
- **No dependency without a measurement** of what it costs a Worker's bundle.
- **Honest status.** Each repository says how far it can be trusted, and
  what changed, release by release.

## Libraries

| library | what it does | status |
| --- | --- | --- |
| [underfetch](https://github.com/workeryard/underfetch) | HTTP over raw sockets: proxies, TLS in WebAssembly, HTTP/1.1 and HTTP/2, and a handshake that can look like a browser | [0.1.0](https://www.npmjs.com/package/@workeryard/underfetch), experimental |

---

WorkerYard is not affiliated with or endorsed by Cloudflare, Inc. Cloudflare
and Cloudflare Workers are trademarks of Cloudflare, Inc.
