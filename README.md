# DeepSeek experiment data — 2026-09-29

[Download the dataset snapshot](https://github.com/Siyuexi/manyi-deepseek-data/releases/tag/snapshot-2026-09-29)

21 data parts plus the index and instructions; total download size 29.49 GB.

Standalone DeepSeek dataset snapshot. The main model is DeepSeek; AgentDiet's configured GPT-5-mini auxiliary records remain part of that method's data. No separate GPT/Claude experiment matrix is included. Attempts excluded by the existing model-scope inventory are listed in EXCLUDED-ATTEMPTS.json.

The existing inventory contains **557/565 scored method–task pairs** (113 tasks × 5 methods), across **846 retained historical/current attempt directories** from 10 runs. Failed unscored attempts are retained. RESULTS.csv and STATUS.json report the inventory snapshot; this export did not rerun experiments, model audits, validation, or download checks.

Includes native trajectories, sessions, request/response records, logs, configurations, submitted patches and evaluation results selected by the existing export rules. Credential/private-identity text is redacted during export. Workspace/dependency trees, runtime caches and redundant expanded accounting/rendered files are omitted; see EXCLUDED-PATHS.json. Source data is unchanged.

## Download and restore

Download **all deepseek-data-20260929-objects-*.zip parts**, **deepseek-data-20260929-index.zip**, and **restore.py** into one directory, then run:

```bash
python3 restore.py --archives . --output restored
```

Python 3.9+; standard library only. These ZIPs form a deduplicated object archive; restore.py reconstructs the original relative file paths. They are not ordinary sequential ZIP volumes. Optional `--prefix runs/RUN_NAME/` restores just one run.

Logical files: 614,137. Unique objects: 557,729. Full decoded logical size: 126,524,756,150 bytes (restoration needs more disk space than download).
