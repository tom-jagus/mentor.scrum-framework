# 📌 Definition of Ready & Done

“Ready” and “Done” are not labels — they’re contracts.  
They define the entry and exit criteria for work at every level of the delivery process.

This document explains what those terms mean, where they apply, and how they are implemented across different work items.

---

## 🎯 Purpose

- Ensure that only well-defined work enters the sprint
- Prevent half-finished or unclear work from being marked complete
- Create consistent expectations across refinement, planning, execution, and review
- Support accountability and confidence in delivery

---

## 🧭 When Do These Definitions Apply?

| Phase                 | What Gets Checked                           |
| --------------------- | ------------------------------------------- |
| Strategic Refinement  | Are Epics and Features Ready to break down? |
| Functional Refinement | Are Stories Ready for Planning?             |
| Sprint Planning       | Are Stories marked `Ready` truly ready?     |
| Daily Execution       | Are Tasks `Done`, or just stopped?          |
| Sprint Review         | Are Stories truly complete and validated?   |

---

## ✅ What “Ready” Means

Work marked “Ready” must:

- Be clearly defined and documented
- Have a known owner
- Contain no blockers or unresolved questions
- Be feasible within the planned scope and timebox
- Be approved by the responsible role (Scope Lead, Coordinator, Analyst, etc.)

---

## 🏁 What “Done” Means

Work marked “Done” must:

- Be fully delivered and tested (if applicable)
- Meet all acceptance criteria or definition of success
- Be reviewed or validated by a second party (Analyst, peer, or stakeholder)
- Have all sub-tasks completed or resolved
- Be reflected in the board status and Sprint Review

---

## 📐 Summary by Work Item

| Work Item      | ✅ Ready Checklist Highlights                                     | 🏁 Done Checklist Highlights                                    |
| -------------- | ----------------------------------------------------------------- | --------------------------------------------------------------- |
| **Project**    | Business outcome defined, aligned with PO, Epics scoped           | All Epics delivered, goal validated, PO confirms                |
| **Epic**       | Linked to Project, outcome clear, at least 1 Feature drafted      | All Features complete, outcome confirmed, closed by Coordinator |
| **Feature**    | Supports Epic, scoped for 1–2 sprints, value clear                | Stories delivered, value demonstrated, confirmed                |
| **User Story** | Linked to Feature, testable, no blockers, acceptance criteria set | All Tasks done, AC met, validated in Review                     |
| **Task**       | Linked to Story, scoped to 1 day, assigned                        | Action completed, code/test delivered, reviewed                 |
| **Bug**        | Reproducible, impact clear, Analyst-approved                      | Fix implemented, validated, marked `Resolved`                   |

This table summarizes only the key points — full checklists live in each work item’s documentation.

---

## 🧠 Best Practices

- Use these definitions actively during ceremonies — not just after the fact
- Refuse to pull work into Planning if it’s not Ready
- Don’t close anything that hasn’t been validated
- Align on “what Done looks like” before work begins

---

## 🚫 Anti-Patterns

- Marking items as `Done` just because all Tasks are finished
- Accepting vague work into the sprint to “figure it out later”
- Confusing technical completion with functional validation
- Skipping review or validation because “we already know it works”

---

## ❓ FAQ

**Q: Who decides when something is Ready?**  
The role responsible for that work item (Scope Lead for Stories, Coordinator for Features, etc.)

**Q: What if a Story is technically complete but not validated?**  
It’s not Done. It must pass functional validation before being closed.

**Q: Do we need full documentation for something to be Done?**  
Only if documentation is part of the Story’s acceptance criteria or required for downstream users.

**Q: Can we bypass “Ready” if the team is confident?**  
No. If something isn’t Ready, it adds risk — even if it _feels_ clear.

---

“Ready” prevents chaos. “Done” builds trust.  
Use both to deliver with confidence — not just completion.
