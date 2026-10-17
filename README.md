# Repolex Knowledge Graph of adafruit/Adafruit_Python_PureIO

RDF knowledge graph data for [adafruit/Adafruit_Python_PureIO](https://github.com/adafruit/Adafruit_Python_PureIO), parsed by [repolex](https://repolex.ai).

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
rlex download adafruit/Adafruit_Python_PureIO
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── bc28777ee0a2b5b4ef51214fb3148dd6bad3f611
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── bc28777ee0a2b5b4ef51214fb3148dd6bad3f611
│           └── chunk-001.nq.gz
├── blob
│   ├── 0dd730085ab5016df3002bd70d0e5cbd0d50855c.nq.gz
│   ├── 1386acf0929968bea3592ed69970f0478cac561b.nq.gz
│   ├── 1d8b8ed52b4b2aa9a6cc85062efbce21945e8e4d.nq.gz
│   ├── 204b93da48d02900098ced21c54062ffbff36b9c.nq.gz
│   ├── 24a8f9019938ba762d40975394d33d2895e8ee4d.nq.gz
│   ├── 3813eabc09971b8692cab43eec517375d9bbf335.nq.gz
│   ├── 3b83f4700a3add122f86b6bdb2e06cc00f9091d4.nq.gz
│   ├── 3f92dfc5fdda05635f28da16a47fa1a5c99c0dc6.nq.gz
│   ├── 451c87013a6ad0783f6bd92ea91baced3bc91b49.nq.gz
│   ├── 5aca98376a1f7e593ebd9cf41a808512c2135635.nq.gz
│   ├── 60b5512397168aadc71610ef0f6db2976ee54862.nq.gz
│   ├── 7ab9f83aa13abf21510cfe0213569640e39ee58e.nq.gz
│   ├── 7ae8226e8499ddd582fc1de14f3b6db0399dc0f9.nq.gz
│   ├── 86a3fbfe831f22cc8a8de7ed0db1c648b2a3fd10.nq.gz
│   ├── 8780e3d705326af045abbdcafca67f1bc54fa021.nq.gz
│   ├── 8f3dfe1f8bb51440b30c935498a5bbd8289abe78.nq.gz
│   ├── 9c047856eef4c6a0c77db011b0c24d3d20191045.nq.gz
│   ├── a2233fac5c2f9291e10ec0603ff1d4017e50e2f5.nq.gz
│   ├── aa6d19278a9e45257dedbfe30f5ff88634a36d8f.nq.gz
│   ├── b3bea754ef6499a02bbd2ee02e440b6aabed521e.nq.gz
│   ├── c5fea908c746111a426ba54ec1df34d25a218d25.nq.gz
│   ├── ccef8015d729e05fccaa84c53f5041eb15a950d7.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── eb09c6ff40c8e34c99fc15328f43bba355dcb617.nq.gz
│   ├── ec1b7b3da5f1422403ba81549e2f4a381b623ff3.nq.gz
│   └── f83e71606db0d446d9668a0e4fe80ee985d566e2.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── bc28777ee0a2b5b4ef51214fb3148dd6bad3f611.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 34 files
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

[adafruit/Adafruit_Python_PureIO](https://github.com/adafruit/Adafruit_Python_PureIO)

---
*Parsed on 2026-10-17 by [repolex](https://repolex.ai)*
