# 📘 Scrum Framework Blueprint

This document defines the operating model for an agile, cross-functional data and reporting team transitioning from a legacy, waterfall-style workflow. It establishes clear roles, work item structures, ceremonies, and processes to enable iterative delivery, reduce chaos, and promote clarity, autonomy, and accountability.

It is intended to be a living reference for all team members — from Product Owner to Developers — and should be refined as the team matures.

## 1. 👥 Roles & Responsibilities

| Role                  | Responsibilities                                                                                                                                                                                                                                                                                                                                                                        |     |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
| **Product Owner**     | Owns the strategic direction of the product and defines high-level project priorities and delivery goals. Provides clear vision and context for the work, ensuring alignment with business needs. Validates outcomes based on stakeholder expectations and evolving organizational objectives.                                                                                          |     |
| **Scope Coordinator** | Translates the Product Owner's strategic vision into a structured backlog of Epics and Features. Maintains and prioritizes the backlog to reflect evolving priorities and sprint goals. Provides ongoing guidance and collaboration to Scope Leads, ensuring alignment across teams and consistent delivery progress. Facilitates backlog clarity and cross-team coordination.          |     |
| **Scrum Master**      | Champions the team's adoption of agile practices by guiding adherence to the framework. Facilitates all Scrum ceremonies with consistency and purpose. Monitors team dynamics and process health, identifying areas for continuous improvement. Actively works to remove framework-level impediments and supports team focus. Mentors team members toward future Scrum Master rotation. |     |
| **Scope Lead**        | Leads the decomposition of Features into well-formed User Stories with assistance from Product Developers. Collaborates closely with the Scope Coordinator to maintain alignment on sprint goals and delivery expectations. Oversees progress within the sprint, ensures delivery readiness, and presents completed work during Sprint Reviews.                                         |     |
| **Product Developer** | Takes ownership of User Stories selected during Sprint Planning and breaks them into actionable Tasks. Designs and implements technical solutions, documents logic, and performs unit testing. Maintains the Scrum board by updating progress and raising blockers. Participates actively in all Scrum ceremonies.                                                                      |     |
| **Product Analyst**   | Clarifies needs with consumers and gathers feedback to inform development. Supports delivery validation by testing functionality and reporting defects. Verifies that acceptance criteria are met and assists in quality assurance. Acts as the first line of support and guides users in the effective use of delivered solutions.                                                     |     |

---

## 2. 🛠️ Work Items & Structure

| Level | Work Item      | Description                                                                                                                                                                                                            | Owner(s)                            |
| ----- | -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| 1     | **Project**    | A high-level initiative introduced by the Product Owner in response to a specific business challenge or opportunity. Projects define the strategic context for delivery and group all related Epics.                   | Product Owner                       |
| 2     | **Epic**       | A major outcome or conceptual component required to complete a Project. Epics define large-scale deliverables that represent a significant shift or advancement toward the Project’s goal.                             | Scope Coordinator + Scope Lead      |
| 3     | **Feature**    | A specific milestone or functional goal that contributes to the completion of an Epic. Features organize related work into coherent objectives that deliver incremental value.                                         | Scope Coordinator + Scope Lead      |
| 4     | **User Story** | A clearly defined unit of functionality that contributes to a Feature. User Stories describe meaningful pieces of work from a stakeholder or implementation perspective, supporting iterative planning and delivery.   | Scope Lead + Product Developer      |
| 5     | **Bug**        | A formally reported defect that affects functionality in a delivered or production-facing solution. Bugs are always tracked at the same level as User Stories and require thorough documentation and rapid resolution. | Product Developer + Product Analyst |
| 6     | **Task**       | A discrete, actionable step taken to fulfill a User Story. Tasks reflect concrete technical or analytical actions and are small enough to be completed within a working day.                                           | Product Developer                   |

- **Azure DevOps Board Columns**: These columns reflect the lifecycle of work during a sprint and enable team-wide visibility and status tracking:

  - `To Do`: Work that is ready to begin, prioritized and committed for the current sprint.
  - `In Progress`: Work that is actively being developed.
  - `Blocked`: Work that cannot proceed due to a dependency, missing input, or external issue. Must be flagged and resolved quickly.
  - `In Review`: Work that is completed by the developer and pending testing, review, or validation.
  - `Done`: Work that meets the Definition of Done, reviewed and accepted.

- **Project Checklist**:

  - Clearly describes a business challenge or opportunity.
  - Has a defined strategic intent or value.
  - Is initiated and validated by the Product Owner.
  - Contains sufficient context to begin Epic definition.

- **Epic Checklist**:

  - Describes a major outcome or conceptual building block.
  - Linked to a specific Project.
  - Approved by both the Scope Coordinator and Scope Lead.
  - Outcome is measurable or clearly verifiable.

- **Feature Checklist**:

  - Supports a defined Epic and delivers tangible value.
  - Sized to fit within 1–2 sprints.
  - Contains a description that outlines scope and success conditions.
  - Reviewed and agreed upon by the Scope Lead and Scope Coordinator.

- **User Story Checklist**:

  - Describes a specific need or problem to solve.
  - Clearly contributes to the Feature’s goal.
  - Has acceptance criteria defined.
  - Is small enough to estimate and complete within a sprint.
  - Reviewed by both the Scope Lead and the assigned Product Developer.

- **Task Checklist**:

  - Linked directly to a User Story.
  - Describes a discrete technical or analytical step.
  - Can be completed within one working day.
  - Contains necessary technical detail or inputs.
  - Is owned and updated by the assigned Product Developer.

---

### 2.1 📊 Role-Based Board Setup

Different roles in the team require tailored visibility into work items and progress. The following board configurations are recommended to support role-specific needs and responsibilities:

#### 🔹 Product Owner View

- **View Type**: Tree or dashboard summary
- **Visible Levels**: Projects, Epics (with rolled-up status of Features and Stories)
- **Purpose**: Strategic oversight without low-level detail. Helps track delivery progress against initiatives.

#### 🔹 Scope Coordinator View

- **View Type**: Tree structure with roll-up metrics
- **Visible Levels**: Projects, Epics, Features (with aggregate progress from Stories and Tasks)
- **Purpose**: Ensures alignment between strategic priorities and planned delivery. Enables refinement and prioritization of Epics and Features.

#### 🔹 Scope Lead View

- **View Type**: Hybrid (Tree + Kanban Board)
- **Visible Levels**: Epics, Features, User Stories (with numeric completion for Tasks)
- **Purpose**: Facilitates sprint planning, User Story refinement, and progress tracking during the sprint. Provides clear visibility into delivery readiness.

#### 🔹 Product Developer View

- **View Type**: Kanban Board
- **Visible Levels**: Features (optional), User Stories, Tasks
- **Purpose**: Daily work management. Helps track active Tasks, flag blockers, and maintain clear focus during execution. Used in Daily Standups.

Each board configuration should be backed by saved queries or views in Azure DevOps that match the scope and granularity appropriate to each role.

---

### 2.2 🧭 Work Item Statuses by Level

Each work item type has its own set of status stages to reflect where it stands in its lifecycle and what attention it may require. These statuses support clarity, ownership, and efficient delivery across all levels.

#### 🔹 Project Statuses

- **Draft** – Initial concept submitted but not yet reviewed
- **Proposed** – Under discussion or review for prioritization
- **Approved** – Validated by the Product Owner and scheduled for delivery
- **In Progress** – Work has begun on related Epics
- **Complete** – All related Epics have been delivered

#### 🔹 Epic Statuses

- **Draft** – Idea created, outcome not fully defined
- **Needs Refinement** – Outcome not measurable or missing acceptance criteria
- **Ready** – Fully defined, linked to a Project, and accepted by Scope Coordinator
- **In Progress** – Work underway on linked Features
- **Complete** – All Features delivered and Epic outcome achieved

#### 🔹 Feature Statuses

- **Draft** – Created but lacking clarity or alignment
- **Needs Clarification** – Ambiguities or missing scope require further review
- **Ready** – Sized for 1–2 sprints and properly defined
- **In Progress** – Actively being refined into User Stories or under implementation
- **Complete** – All linked Stories completed and goal achieved

#### 🔹 User Story Statuses

- **Needs Grooming** – Added to backlog but incomplete or unclear
- **Ready** – Acceptance criteria clear and feasible within sprint
- **In Progress** – Actively being worked on by the team
- **In Review** – Development done, pending validation
- **Done** – Reviewed, validated, and meets Definition of Done

#### 🔹 Task Statuses

- **Ready** – Ready to start with inputs and clarity available
- **In Progress** – Work actively underway
- **Blocked** – Blocked by dependency or missing information
- **In Review** – Implementation complete and being validated
- **Done** – Task completed, tested, and committed

These statuses are used to guide board design and work visibility for each role, supporting timely decision-making and proactive backlog management.

### 2.3 🐞 Bug Handling and Lifecycle

\[previous content retained for context]

---

### 2.4 🔁 Backlog Governance

> 🔸 **Note:** In the current team structure, a Feature often represents the delivery target for a sprint. Therefore, the Feature selected for a sprint typically becomes the implicit **Sprint Goal** unless otherwise defined.

Each work item level has an explicitly defined owner responsible for keeping its portion of the backlog healthy, prioritized, and actionable. Assistive roles help refine and improve items but the primary accountability always remains with the owner.

#### 🔹 Role-Based Backlog Responsibility

| Work Item  | Owner (Primary)   | Supports          |
| ---------- | ----------------- | ----------------- |
| Project    | Product Owner     | None              |
| Epic       | Scope Coordinator | Scope Lead        |
| Feature    | Scope Coordinator | Scope Lead        |
| User Story | Scope Lead        | Product Developer |
| Bug        | Product Developer | Product Analyst   |
| Task       | Product Developer | None              |

#### 🔹 Governance Expectations

- **Ownership = Accountability**: If a work item exists in the backlog, its primary owner is responsible for its clarity, refinement status, and prioritization.
- **Assist = Refine, Not Drive**: Supporting roles provide technical input or downstream clarity but do not make final decisions about content, order, or structure.
- **Visibility is Mandatory**: Items that are stale, unclear, or abandoned must be flagged by the Scrum Master and revisited during ceremonies.
- **No Orphaned Items**: Every item in the backlog must have an assigned owner and be part of the team’s delivery vision.
- **Structured Reviews**: During Strategic and Functional Refinement sessions, Scope Coordinator and Scope Leads audit and realign items as part of governance.

This structure encourages ownership discipline, avoids clutter, and ensures a growing but manageable and meaningful backlog that fuels delivery.

### 2.5 🧱 Work Type Classification

In addition to formal project delivery, the team handles various types of work outside defined Projects, Features, or Stories. These include maintenance, consumer support, exploratory analysis, and ad hoc requests. To maintain clarity while respecting Product Owner boundaries, the following classification and handling suggestions are provided:

#### 🔹 Work Types and Handling Suggestions

| Work Type           | Description                                                            | Suggested Handling                           |
| ------------------- | ---------------------------------------------------------------------- | -------------------------------------------- |
| Project Work        | Items contributing directly to Project-Epic-Feature structure          | Use standard hierarchy (Project → Task)      |
| Bug Fixes           | Defects in production                                                  | Use Bug work item                            |
| Exploratory Work    | Research, spikes, proof-of-concept efforts                             | Use User Story or separate label/tag         |
| Consumer Assistance | Helping users with exports, ad hoc data prep, minor troubleshooting    | Use Task or add "Support" tag under Story    |
| Maintenance         | Operational routines (refresh issues, environment upkeep, credentials) | Use Task with "Maintenance" tag or swimlane  |
| Internal Training   | Documenting, mentoring, or knowledge sharing sessions                  | Optional: Task or track as internal learning |

#### 🔹 Tracking Notes

- Avoid mixing delivery and support in the same Story.
- Add a dedicated **Support / Maintenance Epic** if volume justifies sprint planning inclusion.
- Track hours or frequency of non-project work to inform future capacity discussions.

This flexible but consistent structure ensures all effort is visible, measurable, and can inform future process or staffing improvements.

### 2.6 📊 WIP Limits & Delivery Metrics

As the team matures, visibility into work-in-progress (WIP) and delivery health becomes increasingly important. Implementing light governance around WIP and delivery metrics can help prevent overloading, reduce context switching, and support continuous improvement.

#### 🔹 Work-In-Progress (WIP) Limits

- **Purpose**: Encourage team focus, limit multitasking, and surface bottlenecks.
- **Suggested Practice**:

  - Define WIP limits per column (e.g. no more than 2 "In Progress" stories per person).
  - Scrum Master monitors and surfaces WIP violations during standups.
  - Review WIP trends in retrospectives to identify patterns.

#### 🔹 Delivery Metrics to Track

| Metric          | Purpose                                                  | Owner / Viewer                  |
| --------------- | -------------------------------------------------------- | ------------------------------- |
| Velocity        | Track total story points or stories delivered per sprint | Scrum Master, Scope Coordinator |
| Cycle Time      | Measure average time from "In Progress" to "Done"        | Scrum Master, Team              |
| Work Type Ratio | Show split between project vs support/maintenance        | Scrum Master, Product Owner     |
| Carryover Rate  | Identify stories/tasks not completed within sprint       | Scrum Master                    |

#### 🔹 Implementation Tips

- Start simple: track metrics manually or via Azure DevOps charts.
- Use trends, not targets — avoid turning metrics into performance tools.
- Discuss key trends monthly or during retrospectives.

This guidance helps create a balanced workload, encourages focus, and informs discussions about realistic planning and process improvement.

---

## 3. ⏱️ Ceremonies & Cadence

| Ceremony                          | Participants                                  | Purpose                                                                                                                                                                                                                             | Notes                                                                                                                                                                                                                                                                                                                                     |
| --------------------------------- | --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Strategic Refinement**          | Scope Coordinator, Scope Leads, Scrum Master  | Review, define, and evolve Epics and Features in alignment with current business priorities and delivery strategy. Focuses on maintaining clarity, scope alignment, and readiness of work items above the User Story level.         | **Weekly, non-negotiable**. Ensures the top of the backlog is continuously groomed and ready for downstream refinement.                                                                                                                                                                                                                   |
| **Functional Refinement**         | Scope Leads, Product Developers, Scrum Master | Refine Features into well-defined, estimable User Stories. Ensures each story is clearly scoped, has defined value, and can be confidently implemented by the team.                                                                 | **Weekly, mandatory**. Ensures Features are consistently translated into actionable User Stories and the middle of the backlog remains clear, structured, and ready for planning.                                                                                                                                                         |
| **Tactical Refinement**           | Product Developers, Scrum Master              | Translate selected User Stories into clear, actionable Tasks. Focuses on execution-level clarity, breaking down complexity, and preparing items for daily workflow.                                                                 | **Mandatory and individual.** Must be performed by each Product Developer immediately after or during Sprint Planning. Ensures that User Stories are translated into executable steps and delivery can begin without delay.                                                                                                               |
| **Sprint Planning**               | All                                           | Plan the upcoming sprint by defining team capacity, reviewing the refined backlog, and selecting User Stories that fit within the team's available effort. Ensure each selected item is well-understood and prepared for execution. | **Held at the end of each sprint, prior to the Review.** Sprint scope is determined based on \~80% of team capacity to allow buffer for blockers, support, and unexpected complexity. Planning at this point ensures that no new work is introduced mid-sprint, and the team can start the new sprint with a clean slate and clear focus. |
| **Daily Standup**                 | All                                           | Brief daily check-in to maintain team alignment, track progress, and surface any blockers. Focused on work visibility and delivery momentum.                                                                                        | **Held daily during the sprint.** Discussions are limited to active Tasks. No problem-solving or detailed storytelling—follow-ups are handled separately. Scrum board is used to guide the conversation.                                                                                                                                  |
| **Sprint Review & Retrospective** | All + Product Owner                           | Review completed User Stories from the current sprint, gather feedback, and ensure alignment with sprint goals. Close the sprint by briefly reflecting on what worked and what could improve.                                       | **Held at the end of each sprint.** Scope Lead presents the work. A 5-minute retrospective is conducted at the end of the session to identify quick lessons and improvements.                                                                                                                                                             |

Optional: async mid-sprint progress post (not formal checkpoint)

---

## 4. 🔄 Sprint Flow (2-week cadence)

The following flow outlines the structured rhythm of a 2-week sprint cycle. Each step aligns with the ceremonies defined earlier and ensures that planning, refinement, execution, and review happen in a predictable and productive cadence.

**1. Strategic & Functional Refinement (Week 1 & 2, ongoing)**

- Strategic Refinement held weekly: Scope Coordinator + Scope Leads review and refine Epics and Features.
- Functional Refinement held weekly: Scope Leads and Product Developers define and size User Stories.
- Scrum Master ensures both ceremonies occur and output remains actionable.

**2. Sprint Planning (End of current sprint)**

- All roles participate to define capacity and select refined, ready User Stories.
- Scope is planned to \~80% capacity to allow for unexpected work.
- Product Developers take ownership of User Stories.

**3. Tactical Refinement (During or immediately after Sprint Planning)**

- Each Product Developer breaks down assigned User Stories into Tasks.
- Scrum Master facilitates and ensures work is broken down clearly.

**4. Sprint Execution (Full 2 weeks)**

- Daily Standups are held to track Task-level progress and surface blockers.
- Tasks move across board statuses: Ready → In Progress → In Review → Done.
- Product Analysts validate deliverables progressively.
- Scrum Master ensures blockers are resolved quickly.

**5. Sprint Review & Retrospective (End of sprint)**

- Scope Lead presents completed work to the Product Owner.
- Product Analysts confirm delivery validity.
- 5-minute team retrospective held to identify lessons and improvements.

This sprint flow helps ensure that planning is continuous, delivery is focused, and improvement happens incrementally.

---

### 🗓️ Sprint Calendar Overview

The following table provides a recommended recurring schedule for ceremonies and focus areas across the 2-week sprint cadence. The sprint begins on **Friday (Week 2)**, immediately following Sprint Review & Planning on Thursday. Strategic and Functional Refinement ceremonies are held on the same day and time every week to maintain consistency and reinforce team rhythm. Each ceremony shows its expected duration in parentheses.

| Week / Day | Monday                                               | Tuesday                | Wednesday                                             | Thursday                                                                                                                              | Friday                                |
| ---------- | ---------------------------------------------------- | ---------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| **Week 1** | Daily Standup (15 min) Strategic Refinement (45 min) | Daily Standup (15 min) | Daily Standup (15 min) Functional Refinement (45 min) | Daily Standup (15 min)                                                                                                                | Daily Standup (15 min)                |
| **Week 2** | Daily Standup (15 min) Strategic Refinement (45 min) | Daily Standup (15 min) | Daily Standup (15 min) Functional Refinement (45 min) | Daily Standup (15 min) Sprint Planning (1.5 h) Sprint Review & Retrospective (1 h) Tactical Refinement (30 min, individually by devs) | Sprint Start → Daily Standup (15 min) |

---

## 5. ✅ Definitions & Shared Terminology

Definitions establish shared understanding across the team and ensure work moves forward only when specific quality and readiness criteria are met. These definitions apply to all levels of planning and delivery and support consistency, clarity, and accountability throughout the workflow.

#### 🔹 Definition of Ready

A work item (typically a User Story) is considered **Ready** when it meets all of the following criteria:

- Clearly describes the expected outcome and purpose
- Includes defined and testable acceptance criteria
- Has known dependencies or constraints documented
- References all required data sources or inputs
- Is appropriately sized to be completed within a single sprint

#### 🔹 Definition of Done

A work item (Story or Task) is considered **Done** when:

- All development or implementation work is complete
- It has been reviewed and validated by a Product Analyst
- Associated changes are committed to GitHub (for TMDL-based items)
- Documentation is updated (logic description, usage note, or comment)
- It has been demonstrated in the Sprint Review and accepted by the team

#### 🔹 Definition of Blocked

A work item is considered **Blocked** when it cannot proceed due to an unresolved issue. Blockers must be:

- Clearly identified and noted in the "Blocked" column on the Scrum board
- Escalated to the Scrum Master and/or Scope Lead for resolution
- Reviewed and addressed in the daily standup until cleared.

---

#### 🔹 Additional Terminology

To support consistent understanding and communication, the following terms are used throughout this framework:

- **Acceptance Criteria**: Clear, testable conditions that a work item must meet to be considered complete. Defined during refinement and validated by Product Analysts.
- **Backlog**: The prioritized list of all work items (Projects, Epics, Features, Stories, and Tasks) that represent future or current work for the team. Maintained and curated by the Scope Coordinator.
- **Grooming** (see also "Refinement"): The process of reviewing, clarifying, and improving backlog items to ensure they are ready for delivery. Conducted regularly in Strategic, Functional, and Tactical Refinement sessions.
- **Sprint**: A fixed 2-week timebox during which a set of selected User Stories and Tasks are delivered. Each sprint ends with a Sprint Review & Retrospective and begins with Planning.
- **Work Item**: A generic term used to refer to any unit of work in Azure DevOps (e.g., Project, Epic, Feature, User Story, Task). Each has a clear purpose, owner, and status.
- **Blocked**: A temporary condition where a work item cannot move forward due to an internal or external issue. Requires escalation and resolution.

---

## 6. 🧭 RACI Matrices & Escalation Flow

This section defines clear responsibility boundaries within the team and describes how the team interacts with external roles and escalates blockers. It includes a top-level RACI matrix for internal activities and a second matrix and flowchart for external interactions and escalations.

### 🔹 Internal Team RACI Matrix

| Activity              | Product Owner | Scope Coordinator | Scrum Master | Scope Lead | Product Developer | Product Analyst |
| --------------------- | ------------- | ----------------- | ------------ | ---------- | ----------------- | --------------- |
| Define Project        | A             | C                 | I            | I          | I                 | I               |
| Define Epic/Feature   | C             | A/R               | I            | R          | I                 | I               |
| Refine User Story     | I             | C                 | C            | A/R        | R                 | C               |
| Define Task           | I             | I                 | I            | C          | A/R               | I               |
| Facilitate Ceremonies | I             | I                 | A/R          | C          | C                 | C               |
| Validate Delivery     | I             | I                 | I            | C          | C                 | A/R             |
| Manage Scrum Board    | I             | I                 | A            | C          | R                 | C               |

### 🔹 External Escalation RACI Matrix

| Situation                            | Responsible       | Accountable       | Consulted                | Informed        |
| ------------------------------------ | ----------------- | ----------------- | ------------------------ | --------------- |
| Internal team member is blocked      | Product Developer | Scrum Master      | Scope Lead               | Entire Team     |
| Epic/Feature-level delivery conflict | Scope Lead        | Scope Coordinator | Product Owner            | Scrum Master    |
| Bug reported by consumer             | Product Analyst   | Scrum Master      | Product Developer        | Scope Lead      |
| Priority conflict between projects   | Scope Coordinator | Product Owner     | Scrum Master, Scope Lead | Team (optional) |
| Dependencies outside the team        | Scrum Master      | Scope Coordinator | External Stakeholders    | Product Owner   |
| Major production issue               | Product Analyst   | Scope Lead        | Scrum Master, Developer  | Product Owner   |

### 🔹 Escalation Handling Flow

```
[Issue Detected]
     ↓
[Is it internal?] — No → [Scrum Master logs external dependency]
                                ↓
                        [Scope Coordinator escalates externally]
                                ↓
                          [Track in backlog or status board]
     ↓ Yes
[Is it blocking delivery?] — No → [Resolve in team]
     ↓ Yes
[Raise in Standup]
     ↓
[Scrum Master facilitates unblocking]
     ↓
[Scope Lead supports if issue spans multiple items]
```

---

## Appendix: Suggested Improvements for Future Maturity

As the team grows in agile maturity, consider implementing the following enhancements:

- 🔄 **Onboarding & Role Handover**: Create standard onboarding checklists and guidance for rotating Scrum Master responsibilities.
- ✅ **Sprint Goals Visibility**: Make Sprint Goals explicit, even when tied to a Feature.
- 🧪 **Non-Delivery Work Handling**: Clarify tagging/handling of research, spikes, training, and ad hoc support.
- 📅 **Milestone Planning**: Align long-term roadmap items to Epics and Features where applicable.
- ⛓ **External Dependencies**: Document and track cross-team or 3rd-party dependencies in backlog.
- 🚦 **Escalation Paths**: Define how blockers, delivery conflicts, or planning disputes are resolved.

These improvements are not urgent but should be reviewed quarterly as part of the team’s continuous improvement process.
