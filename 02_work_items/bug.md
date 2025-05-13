# 🐞 Bug

A **Bug** is a reported defect, unexpected behavior, or system failure that prevents a delivered item from functioning as intended. Bugs are treated as first-class work items — tracked, prioritized, resolved, and validated with the same rigor as Stories.

---

## 🎯 Purpose

- Capture issues that impact functionality, stability, or user experience
- Ensure problems are reproducible, traceable, and addressed efficiently
- Maintain quality and trust in the team’s deliverables
- Prevent regressions or unclear rework

---

## 👤 Ownership

- **Primary Owner**: Product Developer (for fix)
- **Supports**: Product Analyst (for validation and triage)

Developers are responsible for resolving Bugs. Analysts ensure Bugs are clearly described, validated, and confirmed prior to resolution.

---

## 📐 Characteristics

- Clearly defines the expected vs. actual behavior
- Reproducible, documented, and linked to affected work
- Sized appropriately — may be fixed in one Task or across several
- Prioritized based on severity, visibility, and business impact
- Can be planned like a Story or handled as part of support rotation

---

## ✏️ Writing Good Bugs

### 🔹 Core Principles

- Be specific — what was expected, what happened, and how to reproduce it
- Include screenshots, logs, test data, or environment info when applicable
- Use objective language — avoid blame or speculation
- Prioritize clarity over completeness if urgency is high

### ✅ Good Examples

- “Breach export CSV omits closed incidents — expected all breaches”
- “Dashboard fails to load when no SLA config is present in dataset”
- “Export button UI disappears on screen resize below 1024px”

### ❌ Bad Examples

- “Fix export issue”
- “Doesn’t work again”
- “Check dashboard problems”

---

## 🔁 Status Lifecycle

| Status        | Description                                                    |
| ------------- | -------------------------------------------------------------- |
| `New`         | Reported, but not yet validated or triaged                     |
| `Confirmed`   | Reproducible and accepted for resolution                       |
| `In Progress` | Currently being worked on by a Developer                       |
| `In Review`   | Fix complete — under Analyst or peer validation                |
| `Resolved`    | Fix confirmed, issue closed, validated in expected environment |

---

## ✅ Readiness Checklist

A Bug is considered **Confirmed** (i.e., ready to fix) when:

- [ ] It is reproducible and clearly documented
- [ ] Expected vs. actual behavior is included
- [ ] Severity and priority are agreed upon by Analyst and Developer
- [ ] Linked to the affected Story, Feature, or release (if applicable)

---

## 🏁 Completion Checklist

A Bug may be marked **Resolved** when:

- [ ] Fix is implemented, committed, and tested
- [ ] Validated by Product Analyst or peer Developer
- [ ] Bug behavior no longer occurs
- [ ] Status is updated on the board and additional regression cases are captured (if needed)

---

## 🧭 Planning Behavior

- High-priority Bugs may interrupt sprint work if blocking business-critical features
- Otherwise, Bugs are estimated, prioritized, and included in the next sprint or support backlog
- Repeat Bugs may signal root cause issues requiring Epics or Features to address fully

---

## 🔍 Board & Visibility

- Bugs move across the board with the same statuses as Stories
- Visible in Sprint Review when critical to delivery
- Bugs must be tracked and reported — silent fixing is not permitted
- Severity tags or swimlanes may be used to triage frequent issues

---

Bugs are signals — not just defects.  
Handled transparently, they protect delivery quality and drive long-term improvement.
