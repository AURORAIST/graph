# graph 历史版本备份

此分支名为 `备份`，保存 `/home/ustc1958/lxy/graph/history` 的代码、文档和小体积实验结果。原有周次目录位于 `history/` 中。

## 备份范围

- 包含筛选后的源代码、脚本、说明文档、指标、曲线、图表和其他小于 100 MiB 的结果文件。
- 排除可重新生成的缓存、Python 字节码、Git 元数据、依赖目录及运行时文件。
- 排除大于或等于 100 MiB 的文件，以及 `stage_outputs` 中可重新生成的中间张量；最终模型或检查点文件仍按大小规则保留。
- 原服务器上的文件保持原样。这是筛选后的备份，并非整个目录的完整副本。

## 清单

- `backup-manifest/included-files.csv`：上传文件、大小和 SHA-256。
- `backup-manifest/excluded-directories.csv`：整体排除的目录，规则适用于其全部子目录与文件。
- `backup-manifest/excluded-files.csv`：单独排除的文件及原因。
- `backup-manifest/summary.json`：本次备份的来源、时间和统计。
