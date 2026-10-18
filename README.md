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
│   │   └── 98195f0d27c3594899feb8d04a47f081959c6ba5
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 98195f0d27c3594899feb8d04a47f081959c6ba5
│           └── chunk-001.nq.gz
├── blob
│   ├── 1a323258f8b1be910a93338f7e80c8e574828b4f.nq.gz
│   ├── 1accf325237c25ff9d6c01a3d1d145183ccb90d7.nq.gz
│   ├── 245434671099cf2e2de9575a0f64dcec837c2b23.nq.gz
│   ├── 254a21e0c0e1758285d6818b9c3c6e3d74847cee.nq.gz
│   ├── 30d9612734d8d5e76642daf3c26dc0121914fefa.nq.gz
│   ├── 345030772441102eda1be73661469a5f726d668a.nq.gz
│   ├── 467bf58e00bf0324c4a89bea2550e0585e6f44bd.nq.gz
│   ├── 4d7fcb4df6650f9cc5f4d22b0c5dcb85c33f918f.nq.gz
│   ├── 5b0e01008c3d3d76f12e8bce95f5a208d1ddc6d5.nq.gz
│   ├── 5d3aab4b9471be0a2836a70e99e5431867094108.nq.gz
│   ├── 68bc17f9ff2104a9d7b6777058bb4c343ca72609.nq.gz
│   ├── 69c4511bd4e0f9d2548ec5945c514022d18ce359.nq.gz
│   ├── 6b5e49b8d08089ce91c4e76a9d565e726442ff6f.nq.gz
│   ├── 7ec568c1136eb8ec86aa05cf7abacfb54c3e5ead.nq.gz
│   ├── 81bf65cc108727f3cd8e7b0a54047d16f31a49ec.nq.gz
│   ├── 822a9a02c3970865e29c5d7ba1c2c73a7ccf3a87.nq.gz
│   ├── 83cf06c1de15e06b524ee6893eee159f699df9d1.nq.gz
│   ├── 9232442458d58ac0a21edbdcf6dfc25ffeb65d6a.nq.gz
│   ├── 92dd33a1a44470e1405a20c617694fd174086fcc.nq.gz
│   ├── 9971f324ad7980f35a647e280aeb8a5f70fd96db.nq.gz
│   ├── 9aa57f2e6bdf2423ca2fbe396a1f8409cb184a83.nq.gz
│   ├── a6722d18b270079fb3da9026c77e68eca0fb906a.nq.gz
│   ├── abfb63bcae770acd015d87029040a0e5e0005f4c.nq.gz
│   ├── acad56395da01b3f084bfd1d03ccea38f7158a87.nq.gz
│   ├── bbddd24f6583cc82abd34fb859e42abbfddbd70e.nq.gz
│   ├── c5d99cd2c3e0d54c5b47e6ba3c5642b7435ab48e.nq.gz
│   ├── c60dd0bec5a36ae592bd29e8a73821b12dc7c1cc.nq.gz
│   ├── ce858b8761d56b5b2e65894a7714fe15c2f80d02.nq.gz
│   ├── db6e2fde8ffab7c6a65d646af1251d1925cbeb7b.nq.gz
│   ├── e0482039fdb874a36651b7c78f3fbf52788cc521.nq.gz
│   ├── e21d1a96e88b87c7a57ccb88adc380daef06d36a.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ede5445292493060bbee70cbe0834c0fba646bcb.nq.gz
│   ├── f164f622c2fb675904484ba0bc3e5c099edcc92a.nq.gz
│   ├── f432eee62e95d17e036c22a7001ed83417d7a645.nq.gz
│   ├── f6f2494471626a1400cb515d7f884cf759ff1365.nq.gz
│   └── fcb1a6db06c53e70d3b19a5000f5868deddfbec3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 98195f0d27c3594899feb8d04a47f081959c6ba5.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 45 files
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
*Parsed on 2026-10-18 by [repolex](https://repolex.ai)*
