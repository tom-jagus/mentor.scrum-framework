# 🐞 Bug Handling

Bugs are first-class work items. They are tracked, prioritized, and resolved with the same discipline as Stories and Tasks — not as side work or invisible debt.

This file outlines how bugs are reported, triaged, validated, and closed across the team.

---

## 🧭 Purpose

- Capture and communicate defects clearly
- Ensure bugs are reproducible, prioritized, and testable
- Enable fast resolution without derailing sprint goals
- Maintain trust in delivered functionality

---

## 🔄 Bug Lifecycle

| Status          | Meaning                                                            |
| --------------- | ------------------------------------------------------------------ |
| **New**         | Bug has been reported but not yet confirmed or prioritized         |
| **Confirmed**   | Analyst or Developer has validated the issue and documented impact |
| **In Progress** | Developer is actively working on a fix                             |
| **In Review**   | Fix is complete and under validation                               |
| **Resolved**    | Bug validated and closed                                           |

Bugs follow the same board flow as Stories and Tasks: `To Do → In Progress → In Review → Done`.

---

## 🛠️ How to Report a Bug

Every bug must include:

- [ ] Summary of the issue (clear and concise title)
- [ ] Steps to reproduce
- [ ] Expected vs. actual outcome
- [ ] Impact or severity (e.g. blocks user, cosmetic issue, incorrect result)
- [ ] Affected system, module, or data set (if applicable)
- [ ] Screenshots or error logs (optional but recommended)

---

## 📊 Bug Ownership

| Phase              | Primary Owner     | Supports                 |
| ------------------ | ----------------- | ------------------------ |
| Reporting          | Product Analyst   | Anyone (via standup)     |
| Validation         | Product Analyst   | Product Developer        |
| Fixing             | Product Developer | —                        |
| Final Verification | Product Analyst   | End user (if applicable) |

---

## 🧪 Severity Levels

| Level         | Description                                           | Handling Recommendation                     |
| ------------- | ----------------------------------------------------- | ------------------------------------------- |
| 🔴 Critical   | Blocks business use or causes data loss               | Fix immediately, may interrupt sprint work  |
| 🟠 Major      | Breaks expected behavior with significant user impact | Prioritized within sprint                   |
| 🟡 Minor      | Cosmetic or low-impact issue                          | Logged, triaged, planned into future sprint |
| ⚪ Suggestion | UX improvement or optimization                        | Logged separately; not tracked as a "bug"   |

Severity is defined collaboratively by the Product Analyst, Developer, and Scope Lead.

---

## ⏱️ Timing & Triage

- New bugs are reviewed during **Daily Standup**
- Confirmed bugs are estimated and assigned as needed
- Critical bugs may interrupt sprint work and require immediate attention
- Minor bugs are grouped into maintenance Features or Support swimlanes

---

## 📁 Documentation & Tracking

- All bugs are stored in Azure DevOps and labeled as `Bug`
- Linked to the affected Story, Feature, or Project whenever possible
- Bugs that require repeated triage should be escalated to the Scrum Master

---

A defect is just another form of work — but one that threatens quality. The faster it's clarified, assigned, and resolved, the more stable and trusted the team’s output becomes.
