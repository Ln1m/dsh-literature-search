# dsh-literature-search

给模型加一个 `literature_search` 工具：一次结构化调用完成文献检索（OpenAlex 按被引排序 + arXiv 按相关度），不必先读技能正文再跑 shell 命令。

## 装

```sh
dsh plugin --profile web add file:<本仓库>
```

装完重启 web 实例。

## 环境变量

| 变量 | 默认 | 说明 |
|---|---|---|
| `DSH_PAPER_SEARCH_SCRIPT` | `~/Research-Tools/paper-search.py` | 后端脚本路径，脚本需自备 |

## 前提

- 本机 `python` 可用（工具用 `python <脚本> <关键词> <条数>` 调用）
