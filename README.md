# Repolex Knowledge Graph of python-trio/exceptiongroup

RDF knowledge graph data for [python-trio/exceptiongroup](https://github.com/python-trio/exceptiongroup), parsed by [repolex](https://repolex.ai).

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
rlex download python-trio/exceptiongroup
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── dd8fe794d54f058c3bf06f4b06f2f5723879209e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── dd8fe794d54f058c3bf06f4b06f2f5723879209e
│           └── chunk-001.nq.gz
├── blob
│   ├── 06524f032f3ea32acbb4db96402633eb2ceb606e.nq.gz
│   ├── 0c70df18405eab83762d7a77df516aafadf19a65.nq.gz
│   ├── 104c402ebf17ef55f9cdca2114f0a4449f6dd039.nq.gz
│   ├── 1fb68df41f88968fdac81f54f0b5654cffe77569.nq.gz
│   ├── 284fcc12bc32e4560a6ec5cd81fcf32880a85e8b.nq.gz
│   ├── 291bfeaa3b207e4173c50080f22cfb473363ee5a.nq.gz
│   ├── 2c71c9d662a8386fb39cb4c7d1bd35c67ea1275e.nq.gz
│   ├── 31c3c9c64f1aae3314c1d3266f259da6ec444ed7.nq.gz
│   ├── 34ea8ef4422989349ea2e7d9ad73f3eb46fa8620.nq.gz
│   ├── 47ad4b1d6f68df976d9c63307c411ebab7daa205.nq.gz
│   ├── 490c03a02a385026c9d8b1f6856cd3845e7d99e2.nq.gz
│   ├── 4edd4b18b3f9a2893c3d0a37e5e747a5f09cebe7.nq.gz
│   ├── 51f3442917839f8e0f0cccb52b3c10968ad0779e.nq.gz
│   ├── 67898ba6f5cffa770a3110d8c996c8203cbbdc26.nq.gz
│   ├── 6dbe3ef1eaec8c43c02e03dbfde4dea35ebe7926.nq.gz
│   ├── 7098011b03dcb6f97777c2b001bdfe7781dae7b9.nq.gz
│   ├── 76179f02348bee7a8a747e2ed717670b81f5e70c.nq.gz
│   ├── 76d68a98b395b4173db0066370d7f03eab741ab9.nq.gz
│   ├── 87e44540d0f6004a5d44bed34fe284ff3224483d.nq.gz
│   ├── 992426bb97f7827d9c337daf13c1fb174cc5b1ba.nq.gz
│   ├── 9955deccd941f6c55582dcec1e96d1caf2e1980f.nq.gz
│   ├── 9b1f6d6139c780bdd1edf06658c984c51de9d848.nq.gz
│   ├── a0ebcada25b2b90821eb35ded4097d1314a916a1.nq.gz
│   ├── a1f6cb598dd0b409ebf27eeb214b058e9c9945aa.nq.gz
│   ├── a380334655ab85e731bf05334949b6241eefaa33.nq.gz
│   ├── a48c2358ad1b161fc03b15392b694d6dedc2ca75.nq.gz
│   ├── b27e2d9498748ae29220b6d2f84e53a19983069a.nq.gz
│   ├── b5a78b4e40bd564942a58852dace99ed2792831d.nq.gz
│   ├── b5c8fe42052a746770080682b669d8b9d951d058.nq.gz
│   ├── b6fd0d6bca5d2925162a4fa6701de6811a683c3d.nq.gz
│   ├── b8af5c62ed87afd5dd7743c4531894aa1b702228.nq.gz
│   ├── b8bb97185926d7daed314609753173945ed4ff1a.nq.gz
│   ├── c30eb344ce9e81000eb9188f3de5dcddd6af9442.nq.gz
│   ├── ce17e25b7aff0f8578c2e1951c343caf9b29b2b2.nq.gz
│   ├── d645695673349e3947e8e5ae42332d0ac3164cd7.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f2cafd1305c2c857fac703e3dd50808c092f17f5.nq.gz
│   └── f38c5167733eb2fd1cb677450f876788a4aa603e.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── dd8fe794d54f058c3bf06f4b06f2f5723879209e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 46 files
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

[python-trio/exceptiongroup](https://github.com/python-trio/exceptiongroup)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
