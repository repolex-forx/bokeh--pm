# Repolex Knowledge Graph of bokeh/pm

RDF knowledge graph data for [bokeh/pm](https://github.com/bokeh/pm), parsed by [repolex](https://repolex.ai).

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
rlex download bokeh/pm
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 0e25efd2146c3e2947c005fa9ff67aff02f2a93f
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 0e25efd2146c3e2947c005fa9ff67aff02f2a93f
│           └── chunk-001.nq.gz
├── blob
│   ├── 04b01c62258d11fc325dc63d64dfceb50dbc8e9c.nq.gz
│   ├── 10ae7a0aac8c7bd6cb5de9274e8321eba7192819.nq.gz
│   ├── 177a36a7f0b9c3172bf0403993b152a4ac5f56e6.nq.gz
│   ├── 1b7ba61296467f6ded86635529181590359f5697.nq.gz
│   ├── 1ef81058725ebec26e8804ca96ba2650e0467736.nq.gz
│   ├── 2482a12b6f5c3d1b8b9fc2e68ec59f1884d42ddc.nq.gz
│   ├── 2a999a3c867d50a17d8684cb532f5aecbd9c2268.nq.gz
│   ├── 2b0b478f06c22aa36120e3266b1e929b72fcb707.nq.gz
│   ├── 30d14019e5a7a1662f9026c5a496066a7f3fc04b.nq.gz
│   ├── 31f08a9d14dc0b7c558e1044239bf3423dc94f4c.nq.gz
│   ├── 33fff8ba9a7e4451bf3251cc405eccc5ffeb5e0b.nq.gz
│   ├── 379f0dfa8667e5bf7d3608df1c2dbe35abef9900.nq.gz
│   ├── 3cbc0c80d69269753786debe027b46a7691fa5bb.nq.gz
│   ├── 493f952d5a2fc69950c2b96374c7691f8ed12054.nq.gz
│   ├── 4ab4ac568452d68f7376d5c0959d164680d03e00.nq.gz
│   ├── 53f37a979594814789b470dff369e67b500d7a4c.nq.gz
│   ├── 59b73790a378eb93eae346d54668372d969fcdfc.nq.gz
│   ├── 5a938a8cbe4fee007625655657353d2e72b53cbf.nq.gz
│   ├── 65d10112acd26ddeeaad6ac6b30f9185bfe76bb9.nq.gz
│   ├── 6b034236f10ce9ef41de8edbf1a0428e5f2aae76.nq.gz
│   ├── 6e42bd4062ac242213acf65770495d1adaf70bf1.nq.gz
│   ├── 72276c25b52e6a3ce81a3208f21073b32a9c5206.nq.gz
│   ├── 7b1c9df28510da49175c172146b9c4cef93ea4aa.nq.gz
│   ├── 7f650a508ddafc4c5c0533352eebcf0a9ed2fe98.nq.gz
│   ├── 8a0da1c58dd8ac20eb42718e86e5690d8aec70a1.nq.gz
│   ├── 8e2a1503ee33f208836f6a404690f002e4af4d48.nq.gz
│   ├── 8fcf5eeac5283fa834e842efe88f4b84abaffd39.nq.gz
│   ├── 902ef275e4536fed265a7a74a5381cf57957a101.nq.gz
│   ├── 9151e5b3f692c43bfa3aa02b74ef42d2e7b968c1.nq.gz
│   ├── 99ad5e746b3be3a0171ad309182cc00cd1699c0c.nq.gz
│   ├── a5b63a2631ad9e24fafd7e6e858f9636ff4a68c5.nq.gz
│   ├── a84ac664da75a9607b345ec1b852642732949420.nq.gz
│   ├── b3930d0f047184047cb81d620436d91653438b8b.nq.gz
│   ├── b790186f3f042e5410079861e4c39a00a32c2411.nq.gz
│   ├── babe28295df717675570b0c6b39dfaba9fe60328.nq.gz
│   ├── bf2638d84f79105a18cdf0e9ca3eab20defb3e41.nq.gz
│   ├── c97317a6998e113d254d82c6f1de8a4bedb8df39.nq.gz
│   ├── dcc6c0a8b8d76340ad1e85f2f26f1c38305144ce.nq.gz
│   ├── de3e08794a99f5078df374cd9455c7e95bdbd1fb.nq.gz
│   ├── e93b3accab4a132db1135e5bc4db328b57f5c010.nq.gz
│   ├── f1ecad01e41492f4cd291c322a983e82b0fa7ae8.nq.gz
│   └── f4ab3a3bf7f6f2a504619fda3bc29752f9b983c2.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 0e25efd2146c3e2947c005fa9ff67aff02f2a93f.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 50 files
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

[bokeh/pm](https://github.com/bokeh/pm)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
