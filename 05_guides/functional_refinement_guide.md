# 📓 Functional Refinement Guide

Functional Refinement translates Features into clearly defined, testable, and sprint-sized User Stories. This guide provides structure for running or participating in these sessions effectively — whether you're a Scope Lead, Developer, or Analyst.

> 📌 This is not just a meeting — it’s a thinking loop that protects sprint focus and ensures delivery readiness.

---

## 🧭 Purpose

- Decompose Features into well-formed User Stories
- Define acceptance criteria and dependencies
- Size Stories appropriately for a single sprint
- Clarify what “done” means _before_ work starts

---

## 👥 Who Participates

| Role                  | Involvement                                             |
| --------------------- | ------------------------------------------------------- |
| **Scope Lead**        | Facilitates session, presents Features, leads breakdown |
| **Product Developer** | Contributes technical insights, estimates complexity    |
| **Product Analyst**   | Helps define acceptance criteria and edge cases         |
| **Scrum Master**      | Ensures process discipline and readiness standards      |

---

## ⏱️ When It Happens

- **Every Wednesday**
- **Duration**: 45 minutes
- **Cadence**: Weekly, during both sprint weeks

---

## 🔁 Session Flow

1. **Preparation (before session)**

   - Scope Lead selects 1–2 Features that are marked `Ready`
   - Stories are pre-drafted or outlined for discussion

2. **Open the session**

   - Confirm participants and session goal
   - Scrum Master reinforces that only `Ready` Stories will pass forward

3. **Decompose Features**  
   For each Feature:

   - Identify user or stakeholder needs
   - Define specific outcomes
   - Break into discrete, deliverable User Stories

4. **Write or validate acceptance criteria**

   - Each Story must be testable and clearly scoped
   - Analyst supports wording and test case coverage

5. **Estimate (if applicable)**

   - Developers assign story points or flag Stories needing more input

6. **Gate check**

   - Apply Readiness Checklist (see below)
   - Move only “Ready” Stories into backlog planning queue

7. **Close out**
   - Recap Stories moved forward
   - Flag items that need follow-up (tech review, external input, PO clarification)

---

## 📋 Story Readiness Checklist

A Story is considered **Ready** when:

- [ ] It clearly describes a specific user need or system behavior
- [ ] It is linked to a Feature
- [ ] It contains well-defined, testable acceptance criteria
- [ ] It fits within a single sprint
- [ ] It contains no unresolved dependencies or unknowns
- [ ] It is understood and agreed on by Developers and Analyst

---

## ✏️ Writing Clear User Stories

### 🔹 Core Principles

- Stories describe _what’s needed_ — not how to build it
- Each Story should solve one user problem or deliver one system outcome
- Must be testable, small, and clearly tied to value
- Avoid assumptions — write for clarity, not memory

### 🔹 Writing Patterns

- **User voice** (for front-end or functional work):  
  _“As a [user], I want to [action] so I can [value]”_

- **System voice** (for backend or technical work):  
  _“Process [source] and output [transformation or result]”_  
  _“Log [error] when [condition] is met”_

- **Validation triggers**:  
  _“Accept if: [condition 1], [condition 2]”_  
  _“Fail if: [edge case]”_

### 🔹 Good Examples

- ✅ “As a manager, I want to download SLA reports as Excel files so I can prepare compliance summaries”
- ✅ “Return only open incidents when querying SLA breach summary”
- ✅ “Log a warning if SLA data is missing from source feed”

### 🔹 Bad Examples

- ❌ “Improve SLA logic”
- ❌ “Refactor metrics module”
- ❌ “Handle edge cases”
- ❌ “Work on export feature”

---

## 🧠 Facilitation Tips (for Scope Leads)

- Open by stating what Feature you're breaking down and why it matters
- Encourage developers to challenge unclear assumptions
- Ask “What would block us from building this?” — and log responses
- Don’t rush readiness — if it’s not clear, it’s not going into Planning

---

## 🔍 Common Anti-Patterns

| Problem                   | Fix                                                             |
| ------------------------- | --------------------------------------------------------------- |
| Story is too large        | Break it into testable outcomes; check time-box vs. sprint size |
| No acceptance criteria    | Draft expected inputs/outputs with Analyst                      |
| Story is really a Feature | Check for multiple users/behaviors/outputs — regroup upward     |
| “We know what it means”   | If it's not written down, it’s not shared understanding         |

---

## ❓ Frequently Asked Questions

**Q: Can we skip writing acceptance criteria if we’re in a rush?**  
A: No — incomplete Stories create mid-sprint delays and disagreements. Criteria = alignment.

**Q: Should we estimate Stories in this session?**  
A: Yes, if possible. Otherwise flag Stories that need offline review and estimate them before Planning.

**Q: What if we disagree on Story size or scope?**  
A: Defer to the Scope Lead for decision, or split the Story and revisit later. Always choose clarity over debate.

**Q: We refined a Story last sprint, but it changed. Do we re-refine?**  
A: Yes — any change in requirements resets readiness. Clarity is always re-validated.

---

## 🧩 Integration with Planning

- Only `Ready` Stories from this session are eligible for Sprint Planning
- Anything partial or unclear is flagged and returned to the refinement queue
- Sprint Planning should never be used to finish Functional Refinement

---

Functional Refinement is how strategy becomes execution.  
The stronger the Story, the smoother the sprint.
