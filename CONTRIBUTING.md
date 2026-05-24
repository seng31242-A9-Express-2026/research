# Contributing Guidelines - A9 Express Research Repository

Welcome to the **Research & Fact-Finding** workspace for **A9 Express**. To maintain an industry-grade project environment and fully comply with the **University of Kelaniya Software Engineering Teaching Unit guidelines**, all team members must strictly follow the data collection, branch protection, and commit workflows outlined below.

---

# 1. Team Composition & Accountability

All research insights, competitor matrix updates, and client interview summaries must map directly to the assigned researchers for peer review and labor tracking.

* **Thevarasa Dayastan** (SE/2022/007)
* **Arulanantham Mathumithan** (SE/2022/015)
* **Vasanthakumar Arushanth** (SE/2022/016)
* **Surenthiran Sathurjan** (SE/2022/035)
* **Ensilirukman Ronald** (SE/2022/042)

---

# 2. Research Branching Architecture

Our repository utilizes a clean, **linear-trunk workflow**. Direct pushes to the stable `main` branch are strictly blocked by GitHub branch protection rules.

All changes must progress through isolated research or correction branches before being merged into `main`.

## Branch Archetypes

### `main`

The locked production branch. It exclusively hosts finalized, peer-reviewed, and supervisor-approved research documents, matrices, and field studies.

### `draft/<research-topic>`

Active workspaces used for collecting and refining ongoing research findings.

Examples:

```bash id="d3c6f1"
draft/competitive-analysis
draft/client-interview-01
draft/user-personas
```

### `fix/7`

Dedicated branches for corrections or revisions identified during reviews or supervisor evaluations.

Example:

```bash id="w5x9q2"
fix/4
```

---

# 3. Main Branch Protection Enforcements

Per repository governance policies established in **Issue #2**, the `main` branch is protected under the following enforcement rules.

1. **Mandatory Pull Requests**
   Direct commits to `main` are prohibited. All contributions must enter through a Pull Request.

2. **Minimum Peer Review Requirement**
   At least **one team member** must inspect and approve the Pull Request before merging.

3. **Stale Review Dismissal**
   Any new commits pushed to an active Pull Request automatically dismiss previous approvals and require re-review.

4. **Enforced Linear History**
   Only the following merge methods are permitted:

   * **Squash and Merge**
   * **Rebase and Merge**

   Traditional merge commits are disabled to maintain a clean and readable repository history.

---

# 4. Commit Message Standard

The repository strictly follows the **Conventional Commits Specification** to ensure clarity, traceability, and professional repository maintenance.

All commit messages must be written in the **imperative mood**.

Examples:

* Use `add` instead of `added`
* Use `summarize` instead of `summarized`

## Structural Format

```text id="q8m1z4"
<type>(<scope>): <short imperative summary>

[Optional body detailing the analytical context behind the contribution]

[Optional footer linking back to the Kanban board ticket]
```

---

## Approved Commit Types (`<type>`)

| Type    | Purpose                                                                         |
| ------- | ------------------------------------------------------------------------------- |
| `docs`  | Reports, markdown files, research summaries, interview notes, and documentation |
| `feat`  | New research modules, demographics, or analytical sections                      |
| `fix`   | Corrections to data, formatting, spelling, or analytical inaccuracies           |
| `chore` | Workflow maintenance, templates, `.gitignore`, or repository configuration      |

---

## Approved Repository Scopes (`<scope>`)

| Scope      | Usage                                                           |
| ---------- | --------------------------------------------------------------- |
| `pitch`    | Elevator pitches, proposal slides, and panel approval materials |
| `research` | Competitor studies, market analysis, surveys, and fact-finding  |
| `personas` | Stakeholder profiles, user journeys, and customer archetypes    |

---

## Correct Commit Examples

### Competitive Analysis Contribution (Issue #4)

```bash id="m7r2x1"
docs(research): complete competitive analysis for transport platforms

Executes a detailed competitive audit comparing SLTB e-Reservation,
BusSeat.lk, and My Traveller against the A9 Express multi-service
architecture.

Closes #4
```

### Client Interview Findings (Issue #5)

```bash id="n2p4v8"
docs(research): summarize findings from client interview session 01

Compiles structured meeting notes and the finalized requirement questionnaire
from the initial fact-finding session.

Closes #5
```

---

# 5. Kanban Board Tracking Protocol

To maintain transparent project coordination and accurate progress tracking, all contributors must follow the Kanban workflow below.

## Step 1 — Pick Up a Task

Move the assigned issue card from **Backlog** or **To Do** to **In Progress** and assign yourself to the task.

## Step 2 — Open a Draft Pull Request

As soon as your branch is pushed to GitHub, create a **Draft Pull Request** to keep progress visible to both teammates and supervisors.

## Step 3 — Link the Related Issue

Include the following syntax inside the Pull Request description:

```text id="t6u3a9"
Closes #<issue_number>
```

This enables automatic issue tracking and Kanban board synchronization.

## Step 4 — Submit for Peer Review

Once all acceptance criteria are completed:

* Convert the Draft Pull Request into **Ready for Review**
* Request approval from at least one teammate
* Address all review comments before merging

---

# 6. Documentation Quality Standards

All research artifacts submitted to the repository must satisfy the following quality expectations:

* Use professional academic and technical language
* Ensure factual accuracy and source consistency
* Maintain proper Markdown formatting and readability
* Avoid plagiarism and unsupported claims
* Clearly distinguish assumptions from verified findings
* Keep diagrams, matrices, and interview summaries version controlled

---

# 7. Repository Conduct Expectations

All contributors are expected to maintain professional collaboration standards throughout the project lifecycle.

Team members must:

* Participate in constructive peer reviews
* Provide meaningful feedback during Pull Requests
* Maintain respectful communication practices
* Follow repository governance policies consistently

Submissions that fail to meet repository standards may be rejected until the required corrections are completed.
