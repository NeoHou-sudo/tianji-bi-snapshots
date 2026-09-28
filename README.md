# 天玑 · 每日数据快照库（私有）

每个自然日一份数据切片，Git tag 命名 `snap-YYYYMMDD`。

- 结构：`snapshots/data_YYYYMMDD.js.gz`（当日全量看板数据）+ `changes_YYYYMMDD.csv`（与上日差异）+ `metrics.json`（逐日逐经理指标）
- 归档：每晚定时任务自动执行（`archive_snapshot.sh`）
- 取用：`fetch_snapshot.sh YYYYMMDD [目标目录]`
