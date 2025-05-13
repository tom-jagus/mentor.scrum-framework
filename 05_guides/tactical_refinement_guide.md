# 🛠️ Tactical Refinement Guide

Tactical Refinement is the final step before execution. It translates committed User Stories into small, clear, executable Tasks — each scoped to a single day or less.

> 📌 This is a solo activity. Each Product Developer owns their own Tactical Refinement immediately after Sprint Planning.

---

## 🎯 Purpose

- Ensure every Story is fully decomposed into clear, day-sized Tasks
- Eliminate ambiguity before work begins
- Maintain consistent board hygiene
- Prepare the sprint board for execution

---

## 👤 Who Is Responsible

| Role                  | Responsibility                    |
| --------------------- | --------------------------------- |
| **Product Developer** | Breaks down their own Stories     |
| **Scrum Master**      | Verifies completion and readiness |

---

## ⏱️ When It Happens

- **Immediately after Sprint Planning** (same day)
- **Duration**: 30 minutes per developer (self-managed)
- **Cadence**: Every sprint
- **Deadline**: Must be complete _before_ next day's Daily Standup

---

## 🔁 Step-by-Step Process

1. **Review Assigned Stories**

   - Open each Story you accepted during Sprint Planning
   - Confirm that it is marked `Ready`

2. **Break It Down**

   - Create **2–5 Tasks** per Story
   - Each Task should represent 1 day or less of focused work

3. **Write Clear Task Titles**

   - Use action verbs: _“Create…”, “Update…”, “Refactor…”_
   - Make outcomes visible: _“Add validation logic for SLA rules”_

4. **Add Description (if needed)**

   - Include references, known logic, technical notes, or URLs
   - Only if not obvious from the title

5. **Assign Yourself**

   - You are responsible for your own Tasks
   - Use Azure DevOps assignee field

6. **Set Status to `Ready`**

   - All Tasks start in the `Ready` column
   - Do not place anything directly in `In Progress`

7. **Check for Completeness**
   - Every Story must have all Tasks defined and linked before the sprint starts
   - Inform Scrum Master when your refinement is complete

---

## 📋 Task Checklist

Each Task must:

- [ ] Be linked to a single User Story
- [ ] Represent no more than 1 day of work
- [ ] Have a clear, descriptive title
- [ ] Contain any relevant technical info (if needed)
- [ ] Be assigned to yourself
- [ ] Start in the `Ready` column

---

## ✏️ Writing Clear Tasks

### 🔹 Core Principles

- Keep it atomic: one idea, one action
- Name it like a commit message — short and specific
- Use it to track flow — not just to-do lists

### 🔹 Writing Patterns

- _“Build parser for SLA ruleset inputs”_
- _“Refactor timestamp logic to UTC standard”_
- _“Write unit test for data merge case”_
- _“Add error logging for missing records”_

### 🔹 Good Examples

- ✅ “Add export button to dashboard view”
- ✅ “Write test case for empty SLA input”
- ✅ “Validate data feed credentials in staging”

### 🔹 Bad Examples

- ❌ “Do export stuff”
- ❌ “Handle problems with SLA”
- ❌ “Implement logic”
- ❌ “Start working on this”

---

## 🧠 Tips for Developers

- If a Task feels too big — split it
- If a Story is missing detail — escalate it (don’t guess)
- If a Task is done — move it to `In Review` (not `Done`) until validated
- If you block yourself — flag it by moving to `Blocked` and mention it in Standup

---

## ❓ Frequently Asked Questions

**Q: Can I start work before breaking down my Stories?**  
A: No. If the Story isn’t decomposed into Tasks, it’s not ready for execution.

**Q: What if my Story only needs one Task?**  
A: That’s okay — as long as it’s <1 day and clearly named. Otherwise, break it down further.

**Q: Do I need to document each Task in detail?**  
A: Only if it’s not obvious from the name. Keep it clear — not verbose.

**Q: Can I do this later in the week?**  
A: No. All Tactical Refinement must be done **on the same day** as Sprint Planning, before the next Standup.

---

## 📊 Scrum Master Checklist

To verify Tactical Refinement is complete, the Scrum Master checks:

- [ ] All committed Stories have associated Tasks
- [ ] All Tasks are assigned and in `Ready`
- [ ] No Tasks are left vague or misnamed
- [ ] Developers confirmed completion or flagged blockers

---

Tactical Refinement is where planning ends and execution begins.  
No sprint starts until your Tasks are clear.
