# Data provenance and access

Status: no dataset has been approved or uploaded. Complete this record before analysis. Private repository access does not grant permission to redistribute data.

## Source register
| Item | Record before use |
| --- | --- |
| Dataset and provider | Pending selection |
| Official source URL and version | Pending |
| License / data-use agreement | Pending review; record link and restrictions |
| Access approval | Record who may access, approval date, and required training |
| Redistribution | Unverified; do not upload source data |
| Coverage | Dates, hospital/site scope, time zone, sampling, exclusions |
| Unit and schema | Row meaning, field definitions, units, timestamp semantics |
| Target | Arrival count, aggregation interval, forecast horizon |
| Quality | Missing intervals, duplicates, outliers, DST, reporting changes |
| Reproducibility | Retrieval date, source version, local checksum, preprocessing commit |

## Local storage
Keep permitted inputs in data/raw/ and derived files in data/processed/ locally. Both are ignored. Each authorized teammate obtains data independently through the provider's approved process. Never store credentials, patient identifiers, row-level records, restricted extracts, trained artifacts containing sensitive data, or restricted screenshots in GitHub. Do not send restricted data to AI tools.

If access is unavailable, agree an openly licensed aggregate dataset or clearly labeled synthetic demonstration with the instructor. Synthetic results are not evidence of real hospital performance. Do not silently substitute datasets.

## Evaluation controls
Use chronological training, validation, and untouched test periods; record exact boundaries. Fit transformations on training data only. Lag and rolling features must use information available at forecast time. Record missing-data handling and any embargo needed for overlapping horizons. Tune on validation data, not the test set. Report MAE and RMSE against seasonal-naive baselines; define any additional metric before use.

## Sharing review
Before every commit inspect staged files and notebook outputs. Share only permitted, disclosure-reviewed aggregates. Document any small-cell suppression required by the provider. .gitignore is a convenience, not an access-control system; it does not remove already tracked files. If restricted material is committed, stop sharing and follow the provider/institution incident process.
