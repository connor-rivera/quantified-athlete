# quantified-athlete

Personal studies on my own wearable data. I train as a hybrid athlete between the running and resistance training disciplines and wear a Garmin Forerunner 265 and a Whoop 5.0 daily. This repo is where I will turn that data into questions, analyses, and write-ups to gain insights into training and different approaches to augment that training in the most optimal direction for me.

## Studies

| # | Study | Status |
|---|---|---|
| 01 | Garmin vs. Whoop: do two wearables agree on HRV, resting HR and sleep? | Planned |
| 02 | Does shifting to mostly easy running improve aerobic efficiency? (pre-registered) | Pre-registration in progress |

## How it's organized

- 'ingest/': scripts that pull data from Garmin and Whoop
- 'pipeline/': dbt models that turn raw data into clean daily and per-workout tables
- 'studies/': one folder per study, each with its question, methods, results and limitations
- 'data/sample/': synthetic data so anyone can run the code

## Privacy

Raw data, GPS tracks, and account tokens never leave my computer. Only code, daily summaries, charts, and write-ups are published.
