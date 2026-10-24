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
| `rating` | Codeforces problem difficulty rating; blank when unavailable |

## Refresh ratings

Run `python update_ratings.py` with Python 3 (no third-party dependencies).
The script fetches the public [problemset.problems API](https://codeforces.com/api/problemset.problems)
and matches each row by `contest_id` and `problem_index`. It updates `rating`
in place, preserving all other fields and row order. Problems without an API
rating, including problems absent from the response, receive a blank value.

Ratings were fetched on **October 24, 2026**: **11,029** problems have ratings;
**246** are blank (237 matched problems without ratings and 9 unmatched problems).
Ratings reflect the API at refresh time, rather than the statement collection date.

## Notes

- Some optional fields are missing for certain problems, especially `note`, `input_specification`, `output_specification`, and `tags`.
- The `examples` column contains structured sample data.
- This dataset represents the available data **as of September 17, 2026**.
