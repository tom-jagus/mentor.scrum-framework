# 📓 User Story

A **User Story** describes a specific stakeholder need or system behavior that can be delivered within a sprint. Stories are the foundational unit of sprint planning and represent meaningful, testable slices of functionality.

Stories enable the team to focus on value, maintain flow, and validate progress incrementally.

---

## 🎯 Purpose

- Translate Features into discrete, independently valuable units of work
- Deliver something testable, usable, or observable within a sprint
- Serve as the basis for sprint commitment and breakdown into Tasks
- Align team members on outcomes — not implementation

---

## 👤 Ownership

- **Primary Owner**: Scope Lead
- **Supports**: Product Developer, Product Analyst

Scope Leads are responsible for refining Stories until they meet the Definition of Ready, with input from Developers and Analysts to ensure clarity, testability, and feasibility.

---

## 📐 Characteristics

- Written from a user or functional perspective
- Can be completed independently within a sprint
- Describes a clear problem, need, or system behavior
- Contains acceptance criteria that define “done”

---

## ✏️ Writing Good Stories

### 🔹 Core Principles

- Focus on one behavior, action, or outcome
- Use clear, plain language — avoid implementation details
- Include acceptance criteria that are specific and testable
- Avoid bundling multiple behaviors or UI states into a single Story

### ✅ Good Examples

- “As a user, I want to export SLA data so I can prepare compliance reports”
- “Return only open incidents when querying the breach summary endpoint”
- “Log a warning if SLA metadata is missing from incoming feed”

### ❌ Bad Examples

- “Improve SLA logic”
- “Refactor incident service”
- “Handle all dashboard edge cases”

---

## 🔁 Status Lifecycle

| Status           | Description                                       |
| ---------------- | ------------------------------------------------- |
| `Needs Grooming` | Identified, but not yet refined or estimated      |
| `Ready`          | Fully refined, estimated, and ready for Planning  |
| `In Progress`    | Currently under development                       |
| `In Review`      | Work complete, under validation or peer review    |
| `Done`           | Validated and accepted — meets Definition of Done |

---

## ✅ Readiness Checklist

A Story is considered **Ready** when:

- [ ] It is linked to a Feature
- [ ] Clearly describes a user need or system behavior
- [ ] Acceptance criteria are written and testable
- [ ] No open questions, blockers, or unknowns remain
- [ ] Sized to be completed within one sprint
- [ ] Reviewed and approved by Scope Lead and Developer

---

## 🏁 Completion Checklist

A Story may be marked **Done** when:

- [ ] All Tasks are complete
- [ ] The Story meets all acceptance criteria
- [ ] The Analyst (or designated validator) has reviewed the result
- [ ] The Story was demonstrated (or demo-ready) in Sprint Review

---

## 🧭 Planning Behavior

- Only `Ready` Stories are selected during Sprint Planning
- Stories are **not** created during Planning — they must be refined in advance
- Each Developer commits to one or more Stories, which are then broken into Tasks
- Unrefined or blocked Stories are moved out of scope

---

## 🔍 Board & Visibility

- Stories appear on the Scrum board with their status updated daily
- Status moves across: `Ready → In Progress → In Review → Done`
- Tasks underneath each Story reflect granular execution
- Scope Leads and Scrum Master review Story flow and velocity patterns

---

User Stories keep the team focused on _what matters now_ — small, deliverable chunks of value that add up to meaningful progress.
/65/󰍔 /functional_refinement_guide.md
/69/󰍔 /strategic_refinement_guide.md
/70/󰍔 /tactical_refinement_guide.md
