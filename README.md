# Codeforces Problems Dataset

**As of:** September 17, 2026

## Overview

This dataset contains **11,275 Codeforces programming problems** collected in CSV format.

It is suitable for competitive-programming search, problem recommendation, tag analysis, difficulty/contest exploration, and machine-learning experiments.

## File

- `problems.csv` — one row per Codeforces problem.

## Columns

| Column | Description |
|---|---|
| `id` | Codeforces problem ID, e.g. `1A` |
| `contest_id` | Contest identifier |
| `problem_index` | Problem position within the contest |
| `title` | Problem title |
| `time_limit` | Execution time limit |
| `memory_limit` | Memory limit |
| `statement` | Problem statement |
| `input_specification` | Input format and constraints |
| `output_specification` | Required output format |
| `examples` | Sample inputs and outputs |
| `note` | Additional notes, when available |
| `tags` | Comma-separated problem tags |

## Notes

- Some optional fields are missing for certain problems, especially `note`, `input_specification`, `output_specification`, and `tags`.
- The `examples` column contains structured sample data.
- This dataset represents the available data **as of September 17, 2026**.
