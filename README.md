# ER Demand Forecaster

Three-member ML capstone exploring emergency department arrival forecasting and physician staffing scenarios.

**Status:** repository scaffold only. Data access, final target, forecast horizon, model choices, and course requirements remain to be confirmed. No model, results, or operational staffing recommendation is delivered yet.

## Team
| Member | Proposed lead responsibility (confirm together) |
| --- | --- |
| Catarina Torres | Data audit and provenance |
| Maya Gerlach | Modeling and feature experiments |
| Camille Varendonck | Evaluation, uncertainty, and dashboard |

All three members review the analysis, contribute to decisions, and understand the submitted work.

## Project approach
1. Confirm an authorized data source, license, coverage, and aggregation interval in [DATA.md](DATA.md).
2. Define arrival-count target and forecast horizon; audit missing intervals and timestamp quality.
3. Establish naive and seasonal-naive baselines, then compare suitable ML models using chronological validation.
4. Evaluate MAE/RMSE, error patterns, and uncertainty on a held-out future period. Record assumptions and limitations.
5. Explore staffing scenarios only with explicit service-time, physician-capacity, and demand assumptions. Arrivals alone cannot establish safe staffing or patient waiting times. Treat outputs as educational scenarios requiring validation, not clinical guidance.

## Repository map
- src/ — reusable Python code (placeholder).
- notebooks/ — exploratory and experiment notebooks (placeholder guidance).
- evidence/week_10/ through evidence/week_14/ — weekly evidence templates.
- data/ — instructions only; local raw and processed data stay out of Git.
- DATA.md — provenance, access, redistribution, and evaluation controls.
- AI_USE.md — AI assistance disclosure and review log.
- requirements.txt — provisional starter dependencies.

## Local setup
Initial Python target: 3.11; confirm with the course and agree one version as a team.

```bash
git clone https://github.com/catarinaleandro/ER-Demand-Forecaster.git
cd ER-Demand-Forecaster
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter lab
```

On Windows activate with `.venv\Scripts\Activate.ps1` in PowerShell. Repository access requires an accepted collaborator invitation for teammates. Obtain data separately through its approved source; nothing is downloaded by these commands. There is no training command yet.

Dependencies are intentionally unpinned starter suggestions, not a tested environment. Once the first end-to-end run succeeds in a clean environment, record the Python version and freeze exact tested dependencies into a reviewed requirements-lock.txt. Add packages only when used and rerun from a clean environment before submission.

## Team workflow
Create a branch for each task, make focused commits, and open a pull request describing the change and validation. Ask another member to review before merging into main. Keep weekly evidence current and update [AI_USE.md](AI_USE.md) whenever AI assists. Clear notebook outputs containing restricted content before committing; inspect staged changes, including screenshots and attachments.

## First team decisions
Confirm course/group details and deadlines; approve or revise role assignments; verify dataset permission; agree forecast horizon and chronological split dates; assign the first data-audit and baseline tasks. Weekly folders are placeholders, not completed milestones.

## Data and licensing
No datasets are included or approved for redistribution. Private visibility does not override data-use agreements. Read DATA.md before using or sharing any source. No code license is selected yet; confirm ownership and course requirements before choosing one. Any future code license does not license third-party data.
