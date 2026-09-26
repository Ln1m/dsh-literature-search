# dsh-literature-search

[中文](README.md) · English

Adds a `literature_search` tool for the model: one structured call performs a literature search (OpenAlex sorted by citation count + arXiv by relevance) instead of reading a skill body and running a shell command.

## Install

```sh
dsh plugin --profile web add file:<this repo>
```

Restart the web instance afterwards.

## Environment

| Variable | Default | Purpose |
|---|---|---|
| `DSH_PAPER_SEARCH_SCRIPT` | `~/Research-Tools/paper-search.py` | Path to the backend script; you supply the script itself |

## Requirements

- A working `python` on this machine (the tool calls `python <script> <query> <limit>`)
