# KryptLink

URL shortener and click tracker for `kry.li`. The site is inactive for now.

| Implementation | Source | Deployment |
| --- | --- | --- |
| Native Krypton | [`kryptlink/`](kryptlink/) | [Native VPS guide](kryptlink/DEPLOY.md) |
| Node.js | [`kryptlink-node/`](kryptlink-node/) | [Node VPS guide](kryptlink-node/DEPLOY.md) |

Choose one implementation per deployment. Both guides use the same service
name and paths. Keep live databases, passwords, and build output outside the
source checkout. Back up the database before switching implementations.

The native app uses an external Krypton toolchain and stdlib. The Node app
uses Node.js 22.13.0 or newer for `node:sqlite` without an extra flag.
Neither app is part of the Krypton compiler build.

## Source and licensing

The two app directories were moved from
[Krypton at `1030767`](https://github.com/t3m3d/krypton/tree/1030767917c7149d62b40fcac05e26f58fda6968).
Each imported app directory carries its original Apache-2.0 `LICENSE` and
`NOTICE`. The existing root `LICENSE` is unchanged.
