# WorkerYard

Open-source libraries for Cloudflare Workers.

Each one does a thing a Worker's built-in APIs leave out, small enough to read
and checked against the real thing rather than against itself.

| library | what it does | status |
| --- | --- | --- |
| [underfetch](https://github.com/workeryard/underfetch) | HTTP over raw sockets: SOCKS and HTTP(S) proxies, TLS in WebAssembly, HTTP/1.1 and HTTP/2, and a handshake that can look like Chrome, Firefox or Safari | preparing its first release |

## How they are built

- **Measured, not assumed.** A claim about a browser, a server or the platform
  comes with how it was checked, and the check runs again before a release.
- **Reasons written down.** What was taken from other projects, what was left
  out, and why, lives in each repository's `docs/decisions.md`.
- **The runtime at arm's length.** The core takes its socket and its clock
  from the caller; the Workers adapter is one folder, so the rest runs and is
  tested anywhere.
- **No dependency without a measurement** of what it costs a Worker's bundle.

MIT licensed unless a repository says otherwise.

---

WorkerYard is not affiliated with or endorsed by Cloudflare, Inc. Cloudflare
and Cloudflare Workers are trademarks of Cloudflare, Inc.
