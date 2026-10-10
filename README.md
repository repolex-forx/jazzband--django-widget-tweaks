# Repolex Knowledge Graph of jazzband/django-widget-tweaks

RDF knowledge graph data for [jazzband/django-widget-tweaks](https://github.com/jazzband/django-widget-tweaks), parsed by [repolex](https://repolex.ai).

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
rlex download jazzband/django-widget-tweaks
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 483b594c875469827d835941eba4856cec46a5d8
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 483b594c875469827d835941eba4856cec46a5d8
│           └── chunk-001.nq.gz
├── blob
│   ├── 021747e61431f33dabc3dd606053865735e1897d.nq.gz
│   ├── 22270aee1c76a9516406d357825d8379eb889cf7.nq.gz
│   ├── 25125992804ea07d907b7e5bfc3f3cb637227784.nq.gz
│   ├── 377a5274e2e9dea23d3dc43aec399a09dfe38485.nq.gz
│   ├── 41b5011a5d8db6e1cd33f5fa0f1907fd6280ef80.nq.gz
│   ├── 5df841c973a366da6cc9874743accca12910e888.nq.gz
│   ├── 63ce179bf1e0da59aac599a40496aaed39692e8a.nq.gz
│   ├── 68f53df74118c02e72fefdfce11364b2253b497b.nq.gz
│   ├── 69aaac7c1efa7cabf5913352c74b5a04c703404a.nq.gz
│   ├── 84ed47d12b8509744d97884c6d15ba1dedb7a185.nq.gz
│   ├── 86918455f0c99665cf5ca5c79166def19cb87db0.nq.gz
│   ├── 8b5eaa3de66e9ca0afe61ccced42d7c3a7377000.nq.gz
│   ├── 96fee09cced7c27ade726d7bfa5a26062df889af.nq.gz
│   ├── a6f0cdf0c75ac4bd51e87ffd0da5d4ebff2c36c7.nq.gz
│   ├── ad78220bf6ae7568b9e1aff6428f7851beaa7865.nq.gz
│   ├── b87a390733341cd5a1b5df782198288c1db6635f.nq.gz
│   ├── c19d0dcba566c3f00f38da81878e68a2a178fce0.nq.gz
│   ├── e0d5efab56fb94577e7804603eb6f21f36977cb2.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── eb67b2dfec68dbbedb1b08ddffd7489f39839ed0.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 483b594c875469827d835941eba4856cec46a5d8.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 28 files
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

[jazzband/django-widget-tweaks](https://github.com/jazzband/django-widget-tweaks)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
