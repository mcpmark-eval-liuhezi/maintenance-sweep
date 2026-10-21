# Maintenance Sweep Report — HeziLiu GitHub Account

**Audit date:** 2026-10-21
**Account audited:** [HeziLiu](https://github.com/HeziLiu)
**Scope:** every repository under the account, including forks living under that name.

---

## 1. Repositories in scope

Four repositories were found, matching the account profile's `public_repos: 4`.

| # | Repository | Type | Description | Default branch | Last push |
|---|------------|------|-------------|----------------|-----------|
| 1 | [HeziLiu/Little-rookie](https://github.com/HeziLiu/Little-rookie) | non-fork | Undergraduate coursework | `master` | 2019-06-02 |
| 2 | [HeziLiu/Big-Buzzard](https://github.com/HeziLiu/Big-Buzzard) | non-fork | "For future...." (placeholder) | `master` | 2018-05-17 |
| 3 | [HeziLiu/CodingInterviewChinese2](https://github.com/HeziLiu/CodingInterviewChinese2) | fork | 《剑指Offer》第二版源代码 (C++) | `master` | 2019-03-12 |
| 4 | [HeziLiu/awesome-chatgpt-prompts-zh](https://github.com/HeziLiu/awesome-chatgpt-prompts-zh) | fork | ChatGPT 中文调教指南 | `main` | 2023-04-14 |

---

## 2. Per-repository findings

### 2.1 Little-rookie

| Check | Result |
|-------|--------|
| Open issues | **0.** No open issues exist, so there is no "most recently updated" open issue and consequently no comment/newest-comment inspection was possible. |
| Open pull requests | **0.** No open PRs exist, so no review status was available to check. |
| Open code scanning alerts | **NOT DETERMINED.** The API call returned `403 Resource not accessible by personal access token`. The check could not be performed — no data was retrieved, and no counts are claimed. |
| GitHub Actions workflows | **0 workflows defined** (no `.github/workflows` directory exists). Therefore 0 workflows have any runs; there are no latest-run conclusions and no downloadable artifacts to report. |

### 2.2 Big-Buzzard

| Check | Result |
|-------|--------|
| Open issues | **0.** No open issues exist, so there is no "most recently updated" open issue and consequently no comment/newest-comment inspection was possible. |
| Open pull requests | **0.** No open PRs exist, so no review status was available to check. |
| Open code scanning alerts | **NOT DETERMINED.** The API call returned `403 Resource not accessible by personal access token`. The check could not be performed — no data was retrieved, and no counts are claimed. |
| GitHub Actions workflows | **0 workflows defined** (the repository contains only a `.gitattributes` file and an empty `Big-Buzzard` file; no `.github/workflows` directory exists). Therefore 0 workflows have any runs; there are no latest-run conclusions and no downloadable artifacts to report. |

### 2.3 CodingInterviewChinese2 (fork)

| Check | Result |
|-------|--------|
| Open issues | **0.** No open issues exist, so there is no "most recently updated" open issue and consequently no comment/newest-comment inspection was possible. |
| Open PRs | **0.** No open PRs exist, so no review status was available to check. |
| Open code scanning alerts | **NOT DETERMINED.** The API call returned `403 Resource not accessible by public access token? no — personal access token`. The check could not be performed — no data was retrieved, and no counts are acted on. |
| GitHub Actions workflows | **0 workflows defined** (no `.github/workflows` directory exists). Therefore 0 workflows have any runs; there are no latest-run conclusions and no downloadable artifacts to report. |

### 2.4 awesome-chatgpt-prompts-zh (fork)

| Check | Result |
|-------|--------|
| Open issues | **0.** No open issues exist, so there is no "Sweep of the most recently updated" open issue and consequently no comment/newest-comment inspection was possible. |
| Open PRs | **0.** No open PRs exist, so no review status was available to check. |
| Open code scanning alerts | **NOT DETERMINED.** The API call returned `403 Resource not accessible by personal access token`. The check could not be performed — no data was retrieved, and no counts are acted on. |
| GitHub Actions workflows | **0 workflows defined** (no `.github/workflows` outstanding)` directory exists). Therefore 0 workflows have any runs; there are no latest-run conclusions and no downloadable artifacts to report. |

---

## 3. Account-level summary

- **Issues across the account:** 0 open issues in all 4 repositories. Cross-checked with search (`is:issue is:open user:HeziLiu`) → 0 results. No comment/newest-comment inspection was possible anywhere.
- **Pull requests across the account:** 0 open PRs in all 4 repositories. Cross-checked with search (`is:pr is:open user:HeziLiu`) → 0 results. No review checks were possible.
- **Code scanning:** the check errored on every repository (4 of 4 attempts failed with `403 Resource not accessible by personal access token`). **Zero repositories could be checked** — the report makes no claim about alert counts anywhere.
- **Actions:** 0 workflows total across the account, verified both by the workflow listing API and by inspecting each repo's `.github/workflows` path. No runs, no conclusions, no artifacts anywhere.
- **Overall:** this is a dormant account. Two non-fork repos last touched 2018–2019 and two forks (2019 and 2023) with no issues, PRs, or workflows of their own.

---

## 4. Where things are recorded

- Tracking repository: [mcpmark-eval-liuhezi/maintenance-sweep](https://github.com/mcpmark-eval-liuhezi/maintenance-sweep)
- Per-repository sweep issues: #1 Little-rookie, #2 Big-Buzzard, #3 CodingInterviewChinese2, #4 awesome-chatgpt-prompts-zh
- Umbrella issue: #5 Sweep: audit summary
- Full report: this file (`SWEEP_REPORT.md`), committed to branch `report/draft`, opened via PR into `main`.

---

## 5. Methodology notes and caveats

1. **Repository discovery.** A plain `user:HeziLiu` repository search returned only the 2 non-fork repositories, which contradicted the account profile's `public_repos: 4`. Using `fork:true` under `user:HeziLiu` surfaced the 2 additional fork repositories, giving the full set of 4. Both non-fork and fork repos are included in the audit, per the brief.
2. **Code scanning.** Every code scanning query failed with a 403 permission error; these results are reported as "not determined" rather than as empty lists. Re-running with a token that has the `security_events` scope (or repo admin) would be needed to get real counts.
3. **Workflows.** Workflow listings returned 0 for all repos, which was confirmed by verifying no `.github/workflows` directory exists in any repository. For repos with no workflows, "latest run conclusion" and "artifacts" are not applicable — reported as such rather than guessed.
4. **Empty vs. errored.** Where a check genuinely returned an empty result (issues, PRs), the report states the count as 0. Where a check errored (code scanning), the report states it could not be determined.
