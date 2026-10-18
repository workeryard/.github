# WorkerYard

Open-source libraries for Cloudflare Workers.

## Who it is for

Developers building on Cloudflare Workers who reach the edge of what the
platform gives them — a `fetch()` that cannot be pointed at a proxy, a socket
with nothing above it — and need the missing piece done properly rather than
done again in every project.

## Why

A Worker's built-in APIs are deliberately small. What they leave out tends to
be written by hand, once per project, untested against the real thing. Each
library here does one such thing well enough to depend on: small enough to
read, tested without a network, and checked against real servers and real
browsers before a release.

## How

- **Measured, not assumed.** A claim about a browser, a server or the platform
  comes with how it was checked, and the check runs again before a release.
- **Reasons written down.** What was taken from other projects, what was left
  out, and why, lives in each repository's `docs/decisions.md`.
- **The runtime at arm's length.** The core takes its socket and its clock
  from the caller; the Workers adapter is one folder, so the rest runs and is
  tested anywhere.
- **No dependency without a measurement** of what it costs a Worker's bundle.

## Libraries

| library | what it does | status |
| --- | --- | --- |
| [underfetch](https://github.com/workeryard/underfetch) | HTTP over raw sockets: SOCKS and HTTP(S) proxies, TLS in WebAssembly, HTTP/1.1 and HTTP/2, and a handshake that can look like Chrome, Firefox or Safari | experimental, before its first release |

---

WorkerYard is not affiliated with or endorsed by Cloudflare, Inc. Cloudflare
and Cloudflare Workers are trademarks of Cloudflare, Inc.
