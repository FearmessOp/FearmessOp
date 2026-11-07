### Ali Kılıç

Systems and protocol work. Two current projects:

**[agentsig](https://github.com/agentsig-dev/agentsig)** — independent TypeScript
implementation of [IETF Web Bot Auth](https://datatracker.ietf.org/doc/draft-ietf-webbotauth-httpsig-protocol/)
(HTTP Message Signatures, RFC 9421) for Node.js: Ed25519 verification with replay
protection, SSRF-hardened key discovery, lossless RFC 9651 parser, framework adapters.
Six packages on npm; ~5,600 tests pinned to published RFC/IETF vectors. Found a
test-vector inconsistency in the draft
([#135](https://github.com/webbotauth/draft-ietf-webbotauth-httpsig-protocol/issues/135)),
fixed upstream by the spec editor
([#138](https://github.com/webbotauth/draft-ietf-webbotauth-httpsig-protocol/pull/138)).

**[Safrox](https://github.com/FearmessOp/Safrox)** — capability-based x86-64 microkernel
in Rust. Drivers live in ring 3: keyboard IRQ → user-space driver → IPC → console
drawing into the framebuffer, with no kernel code path between the interrupt and the
pixel. Authority is held as capabilities, not inferred from identity — and that
property is tested, not asserted. 72 acceptance scenarios running inside QEMU,
56 architecture decision records.

Interests: Node.js internals, HTTP standards, OS design, making tests prove what
documentation claims.

[npm](https://www.npmjs.com/~fearmessop)
