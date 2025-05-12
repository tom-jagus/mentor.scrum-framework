# 🔄 Non-Project Work

> ⚠️ **Note:**  
> This structure represents a proposed approach to handling non-project work.  
> It is subject to further discussion and refinement by the team before being finalized.

Not all important work fits neatly into a Project–Epic–Feature hierarchy. This file defines how to classify, track, and manage non-project efforts like support, maintenance, and exploration — so they remain visible, measurable, and planned.

---

## 🧭 Why It Matters

- Non-project work is often frequent, high-impact, and time-sensitive
- If left untracked, it distorts planning capacity and masks workload
- By classifying it clearly, the team can plan sustainably and improve visibility

---

## 🗂️ Work Types & Handling

| Type                    | Description                                               | How to Track                                                  |
| ----------------------- | --------------------------------------------------------- | ------------------------------------------------------------- |
| **Bug Fixes**           | Unexpected defects in production                          | Use `Bug` work item type                                      |
| **Consumer Assistance** | Ad hoc requests, data exports, light troubleshooting      | Use `Task` or add `support` tag under active Story or Epic    |
| **Maintenance**         | Regular operational routines, e.g. refreshes, credentials | Use `Task` with `maintenance` tag or a dedicated swimlane     |
| **Exploratory Work**    | Research, prototyping, PoCs                               | Use `User Story` or `Task` with `exploration` label           |
| **Internal Training**   | Mentoring, documentation, onboarding                      | Use `Task`, or group under internal learning Epic if frequent |

---

## 🧱 Organizational Options

Depending on volume and recurrence, non-project work can be structured in one of two ways:

### 🔸 Option 1: Tagged Within Existing Features

- Good for low-frequency or one-off support work
- Tasks are tagged but still live within a sprint Feature
- Useful when work is contextually tied to another Story or Feature

### 🔸 Option 2: Dedicated Swimlane or Support Epic

- Recommended when support/maintenance work is frequent or heavy
- Tasks are grouped under a permanent Epic like `Platform Maintenance` or `User Support`
- Improves long-term tracking and time reporting

---

## 📊 Planning Guidance

- **Estimate** non-project work just like project Tasks
- Include expected support/maintenance time during sprint planning
- Track hours or frequency of non-project work to inform team capacity over time

---

## 🔁 Capacity Adjustments

If non-project work exceeds expected time allocation:

- Surface in Retrospective or Review
- Adjust sprint buffer or limit new Stories in the next sprint
- Propose dedicated support rotations if needed (e.g. “on-call” weeks)

---

## ✅ Summary

| Principle                    | Guideline                                           |
| ---------------------------- | --------------------------------------------------- |
| Visibility is non-negotiable | All non-project work must be logged and tracked     |
| Classify by intent           | Know whether it's support, exploration, or training |
| Size it like project work    | Apply the same estimation and WIP limits            |
| Make it plannable            | Don’t let ad hoc work eat into structured delivery  |

---

Non-project work may be reactive — but it shouldn't be invisible. Tracking it clearly helps the team protect focus, improve estimates, and keep delivery on track.
