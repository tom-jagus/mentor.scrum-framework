# 🧱 Work Items Overview

This section defines the structure, purpose, and lifecycle of all work items used by the team — from high-level Projects to granular Tasks. It exists to ensure every item has a clear owner, meaning, and place in the delivery flow.

Work items are the foundation of planning, tracking, and executing work. Each level serves a distinct purpose, enabling the team to move from strategic goals to daily execution with clarity and control.

---

## 📐 Hierarchy

The team uses a structured hierarchy to break work down across six levels:

| Level | Work Item      | Purpose                                                                   | Primary Owner     |
| ----- | -------------- | ------------------------------------------------------------------------- | ----------------- |
| 1     | **Project**    | Defines the business challenge or opportunity driving high-level outcomes | Product Owner     |
| 2     | **Epic**       | Represents major deliverables aligned to a Project                        | Scope Coordinator |
| 3     | **Feature**    | Groups related functionality or milestones under an Epic                  | Scope Coordinator |
| 4     | **User Story** | Describes a stakeholder need or functional unit of delivery               | Scope Lead        |
| 5     | **Bug**        | Captures a defect impacting expected functionality                        | Product Developer |
| 6     | **Task**       | Represents a concrete, actionable step toward implementing a Story        | Product Developer |

Each item has its own definition, lifecycle statuses, and checklist — detailed in the following files.

---

## 🧭 Ownership & Accountability

Work items are not created in isolation. Each one has a clear **owner** and must serve a defined purpose:

- **Projects** are strategic — owned by the Product Owner
- **Epics** and **Features** are planning layers — shaped by the Scope Coordinator
- **User Stories** are execution-ready — refined and owned by Scope Leads
- **Tasks** are the team’s daily focus — driven by Product Developers
- **Bugs** require fast response — co-owned by Developers and Analysts

Unowned, stale, or unclear items are flagged during ceremonies and cleaned up as part of ongoing backlog governance.

---

## 🔁 Lifecycle & Status

Each work item follows a defined set of statuses, from draft to completion. These statuses:

- Enable board visibility and reporting
- Support accurate forecasting and delivery rhythm
- Clarify what’s ready, what’s blocked, and what’s done

See [`work_item_statuses.md`](./work_item_statuses.md) for full lifecycle breakdowns by item type.

---

## 📊 Work Visibility

All work items are tracked in Azure DevOps, with saved queries and views tailored to each role. Scrum board columns reflect shared delivery stages:

- `To Do` → `In Progress` → `Blocked` → `In Review` → `Done`

See [`board_configuration.md`](../05_tooling/board_configuration.md) for layout guidance and visibility best practices.

---

## ✅ Quality Gates

Each work item type includes a checklist that defines what makes it “ready” or “done.” These checklists ensure that work is not just defined — it’s well-formed, testable, and deliverable.

Checklists are available in [`work_item_checklists.md`](./work_item_checklists.md).

---

## 🧪 Bugs & Exceptions

Bugs are treated with the same structure and discipline as Stories — with their own workflows, ownership, and tracking expectations.

For handling and triage guidance, see [`bug_handling.md`](./bug_handling.md).

---

## 🔄 Non-Project Work

Not all valuable work falls within a Project. Maintenance, support, ad hoc requests, and exploratory efforts are tracked and classified to ensure visibility and sustainable planning.

See [`non_project_work.md`](./non_project_work.md) for classification types and handling practices.

---

This structure allows the team to stay focused, adaptable, and transparent — from long-term initiatives down to daily tasks.
