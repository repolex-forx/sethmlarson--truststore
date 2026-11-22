# Repolex Knowledge Graph of sethmlarson/truststore

RDF knowledge graph data for [sethmlarson/truststore](https://github.com/sethmlarson/truststore), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download sethmlarson/truststore
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 0714f72a739d182cdb8502f4e1bb4cf7ebfe4eb5
│   │   │   └── chunk-001.nq.gz
│   │   └── 98195f0d27c3594899feb8d04a47f081959c6ba5
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 0714f72a739d182cdb8502f4e1bb4cf7ebfe4eb5.nq.gz
│   └── repolex
│       ├── 0714f72a739d182cdb8502f4e1bb4cf7ebfe4eb5
│       │   └── chunk-001.nq.gz
│       └── 98195f0d27c3594899feb8d04a47f081959c6ba5
│           └── chunk-001.nq.gz
├── blob
│   ├── 0166459b40f13bf0f130dc0230af4cb52ea275f9.nq.gz
│   ├── 01f540ba1753feb72d755bf99823ee3b34b80755.nq.gz
│   ├── 1a323258f8b1be910a93338f7e80c8e574828b4f.nq.gz
│   ├── 1accf325237c25ff9d6c01a3d1d145183ccb90d7.nq.gz
│   ├── 245434671099cf2e2de9575a0f64dcec837c2b23.nq.gz
│   ├── 254a21e0c0e1758285d6818b9c3c6e3d74847cee.nq.gz
│   ├── 25f430efaf24638f556fdc7544521efba6deff72.nq.gz
│   ├── 2a515aab6b01c715610d60f10014fa531e78ebc8.nq.gz
│   ├── 30d9612734d8d5e76642daf3c26dc0121914fefa.nq.gz
│   ├── 345030772441102eda1be73661469a5f726d668a.nq.gz
│   ├── 3e25a56773aa5d796581eb41415dda5087eb1460.nq.gz
│   ├── 467bf58e00bf0324c4a89bea2550e0585e6f44bd.nq.gz
│   ├── 47c9a81a335e9e72206122f8c5ef40dae7a42fca.nq.gz
│   ├── 4d7fcb4df6650f9cc5f4d22b0c5dcb85c33f918f.nq.gz
│   ├── 4dada0304c4426cf8e851f4d10668a29a9a993e5.nq.gz
│   ├── 5b0e01008c3d3d76f12e8bce95f5a208d1ddc6d5.nq.gz
│   ├── 5d3aab4b9471be0a2836a70e99e5431867094108.nq.gz
│   ├── 68bc17f9ff2104a9d7b6777058bb4c343ca72609.nq.gz
│   ├── 69c4511bd4e0f9d2548ec5945c514022d18ce359.nq.gz
│   ├── 6b5e49b8d08089ce91c4e76a9d565e726442ff6f.nq.gz
│   ├── 7ec568c1136eb8ec86aa05cf7abacfb54c3e5ead.nq.gz
│   ├── 81bf65cc108727f3cd8e7b0a54047d16f31a49ec.nq.gz
│   ├── 822a9a02c3970865e29c5d7ba1c2c73a7ccf3a87.nq.gz
│   ├── 82fe2029a1f31c07099256e9f0de8c8fce32c2fe.nq.gz
│   ├── 83cf06c1de15e06b524ee6893eee159f699df9d1.nq.gz
│   ├── 8713ce331056edb6a2e87774edad7c4e293f103a.nq.gz
│   ├── 9232442458d58ac0a21edbdcf6dfc25ffeb65d6a.nq.gz
│   ├── 92dd33a1a44470e1405a20c617694fd174086fcc.nq.gz
│   ├── 9971f324ad7980f35a647e280aeb8a5f70fd96db.nq.gz
│   ├── 9aa57f2e6bdf2423ca2fbe396a1f8409cb184a83.nq.gz
│   ├── 9f5aba2374f18bbf267068fdb27074ec77c60099.nq.gz
│   ├── a4623a192dfcdaa2b899d5e92f28247210f90ccf.nq.gz
│   ├── a6722d18b270079fb3da9026c77e68eca0fb906a.nq.gz
│   ├── a7aec30a3f55e86cf9ea6fab28713bd2064c48c8.nq.gz
│   ├── a9bf9abdfc8ed065a2253af17daa07cce4009022.nq.gz
│   ├── abfb63bcae770acd015d87029040a0e5e0005f4c.nq.gz
│   ├── acad56395da01b3f084bfd1d03ccea38f7158a87.nq.gz
│   ├── b1ee7a3cb13a8a3482f2cb8cadef097087e3780b.nq.gz
│   ├── b41e930b212da4dfddf3a4395f075364026c6fa6.nq.gz
│   ├── b663efe85b7f555b195dd38bc2339e934741806a.nq.gz
│   ├── bbddd24f6583cc82abd34fb859e42abbfddbd70e.nq.gz
│   ├── c5d99cd2c3e0d54c5b47e6ba3c5642b7435ab48e.nq.gz
│   ├── c60dd0bec5a36ae592bd29e8a73821b12dc7c1cc.nq.gz
│   ├── ce858b8761d56b5b2e65894a7714fe15c2f80d02.nq.gz
│   ├── db6e2fde8ffab7c6a65d646af1251d1925cbeb7b.nq.gz
│   ├── de181c91e6de29e09f9aaff78950b9335c8b8e67.nq.gz
│   ├── dfdad684e2ce9b2d4bfb3f5629ca94d86b1f61ca.nq.gz
│   ├── e0482039fdb874a36651b7c78f3fbf52788cc521.nq.gz
│   ├── e21d1a96e88b87c7a57ccb88adc380daef06d36a.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ede5445292493060bbee70cbe0834c0fba646bcb.nq.gz
│   ├── ef696173c3cc866d2fd843417c01f8a943789156.nq.gz
│   ├── f164f622c2fb675904484ba0bc3e5c099edcc92a.nq.gz
│   ├── f432eee62e95d17e036c22a7001ed83417d7a645.nq.gz
│   ├── f6f2494471626a1400cb515d7f884cf759ff1365.nq.gz
│   ├── fc5a998c05e6dfe648f8c00ba76100b091284600.nq.gz
│   ├── fcb1a6db06c53e70d3b19a5000f5868deddfbec3.nq.gz
│   └── febc5347cb793a8974623e8c380486418a129bbc.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 0714f72a739d182cdb8502f4e1bb4cf7ebfe4eb5.nq.gz
├── filetree
│   ├── 0714f72a739d182cdb8502f4e1bb4cf7ebfe4eb5.nq.gz
│   └── 98195f0d27c3594899feb8d04a47f081959c6ba5.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

17 directories, 71 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[sethmlarson/truststore](https://github.com/sethmlarson/truststore)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
