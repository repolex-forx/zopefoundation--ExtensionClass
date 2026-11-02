# Repolex Knowledge Graph of zopefoundation/ExtensionClass

RDF knowledge graph data for [zopefoundation/ExtensionClass](https://github.com/zopefoundation/ExtensionClass), parsed by [repolex](https://repolex.ai).

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
rlex download zopefoundation/ExtensionClass
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── b923a0475881072d8fbf22c1e35927a96e3fcf34
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── b923a0475881072d8fbf22c1e35927a96e3fcf34
│           └── chunk-001.nq.gz
├── blob
│   ├── 0a85ce093553b470ba58cb2405114f6d24dd99be.nq.gz
│   ├── 0b0c05a36fcb47581829223bf8b099ac3bc2a24d.nq.gz
│   ├── 1c96442550260eda178e4c38f828582fd680d88e.nq.gz
│   ├── 28779f263b23e88c6824d6e4e35f0d5e641aa02f.nq.gz
│   ├── 4b7e84d4189385d5b6e4f9f483836836c7d6b1e7.nq.gz
│   ├── 58cd1437d31f354fbce1400e2da3f0390f2d30fc.nq.gz
│   ├── 5a528c76594fbac246a8e276e0724ad5c82bde3c.nq.gz
│   ├── 5ed4e606266545d78379b303050e9cda4d2a2e5d.nq.gz
│   ├── 64a6b52ec3240ed9a782ebdf8efe6a150a4fb2c9.nq.gz
│   ├── 668ba873c27d8c74a1e5423e7af624ad1c8b9788.nq.gz
│   ├── 68599d18358a464abea0a8c44cdbe76532c8c018.nq.gz
│   ├── 76cb627dc621977e42b6dab4436fbc840840bc56.nq.gz
│   ├── 77f3c744e601e8cdd746df3914bf9c9c8ea5365f.nq.gz
│   ├── 78609a5f5a06dd7d09bef2926810c672a193b0a1.nq.gz
│   ├── 8aa05e418f941b2328f62e5d7bfe71b7533685f8.nq.gz
│   ├── 8d8dc592df079581db1d871983768d3e84243e3a.nq.gz
│   ├── a4a38a1803b01f191c832128836e48861d4a3612.nq.gz
│   ├── a5a95dfc7730b4b9da3b971f017aec0a7d022002.nq.gz
│   ├── ada2e8515022a89633f433ab6133c0767dd996c0.nq.gz
│   ├── b18520fe62d3f14d74d7baa7359c2fce7d5cba6e.nq.gz
│   ├── b8581dd898cbb33e63961b4d181ff0ffbe5d03ee.nq.gz
│   ├── bab7f94be5ef86cce49612e6cdab326a57143d7d.nq.gz
│   ├── c8383cab9e2f50f4d5dd31ad926833a564860491.nq.gz
│   ├── df8bf084ad61c14baf8d83252f3fafdca2b59996.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e62eec2685820226d926dae3ba92518b526a522e.nq.gz
│   ├── f2357f82cf2720e671c35fe7a8fbd5eb63dfe838.nq.gz
│   ├── f608bcd2bc6de66acd92b3d8aab86a0c80e8d9f1.nq.gz
│   ├── fdafa384691cf7210c388eca5b4069293bc7e205.nq.gz
│   ├── ffe8b620dbbc988ce3cfbca8e5a04c0ae858e29a.nq.gz
│   └── ffee6a163301e8ce55668b2a9bbe412f51a594fd.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── b923a0475881072d8fbf22c1e35927a96e3fcf34.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 39 files
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

[zopefoundation/ExtensionClass](https://github.com/zopefoundation/ExtensionClass)

---
*Parsed on 2026-11-02 by [repolex](https://repolex.ai)*
