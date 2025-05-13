# 🚦 Escalation Handling

Escalation is not failure — it’s a support mechanism. When something is unclear, blocked, or unresolved beyond a developer's scope, it must be raised quickly and visibly.

This process defines when to escalate, who owns the response, and how to track resolution without delay or ambiguity.

---

## 🎯 Purpose

- Ensure blockers and delivery risks are surfaced and addressed quickly
- Clarify how and when to escalate issues inside and outside the team
- Maintain momentum and prevent silent failure
- Reinforce team trust and communication under pressure

---

## 📍 What Should Be Escalated?

| Escalation Type           | Examples                                                             |
| ------------------------- | -------------------------------------------------------------------- |
| **Delivery Blockers**     | Missing data, access issues, failed automation, unclear requirements |
| **Planning Misalignment** | Stories too large, priorities conflicting, scope unclear             |
| **External Dependencies** | Waiting on other teams, systems, or vendor action                    |
| **Repeat Issues**         | Same bug, blocker, or decision gap shows up across multiple sprints  |
| **Priority Conflicts**    | Stakeholders disagree on scope or direction                          |

---

## 🔁 Escalation Flow

```
[Issue Detected]
↓
[Can I resolve this directly?] — Yes → [Resolve, document, and continue]
↓ No
[Raise in Daily Standup or directly to Scrum Master]
↓
[Scrum Master triages]
↓
[Internal or External?]
↓
— Internal: Scrum Master + Scope Lead coordinate fix
— External: Scope Coordinator or Product Owner escalate as needed
```

---

## 👥 Role Responsibilities

| Role                  | Escalation Responsibility                                 |
| --------------------- | --------------------------------------------------------- |
| **Developer**         | Flags blockers early and clearly — never sits silently    |
| **Scrum Master**      | First-line triage, coordinates internal resolution        |
| **Scope Lead**        | Resolves planning or scope issues inside the sprint       |
| **Scope Coordinator** | Escalates to other teams or business contacts if needed   |
| **Product Owner**     | Supports priority clarification and stakeholder alignment |

---

## ⏱️ Escalation Timing

| Type                  | Escalate Within                                 |
| --------------------- | ----------------------------------------------- |
| Critical Blocker      | Same day                                        |
| Planning Misalignment | Before next sprint                              |
| Unresolved Dependency | Within 48 hours                                 |
| Repeated Issue        | Raise during Retrospective or earlier if urgent |

---

## 🛠️ Where to Track Escalations

| Type                    | Tracking Location                                     |
| ----------------------- | ----------------------------------------------------- |
| Blocked Task or Story   | Azure DevOps — move to `Blocked`, add context comment |
| Cross-team dependency   | Azure DevOps or shared doc — tag and track status     |
| Escalation requiring PO | Mentioned in Sprint Review or Planning summary        |

---

## ✅ Best Practices

- Escalate early — don’t wait for blockers to resolve themselves
- Use facts, not blame — escalate the issue, not the person
- Escalate visibly — silent blockers slow the entire team
- Document context clearly — avoid repeating discussions

---

## 🚫 Anti-Patterns

- Waiting days to flag a blocker
- Raising issues verbally but not tracking them
- Escalating around team structure instead of through it
- Assuming someone else already flagged the problem

---

## ❓ FAQ

**Q: I’m blocked but unsure who can resolve it. What should I do?**  
Raise it in Daily Standup. The Scrum Master will help triage or find the right contact to support you.

**Q: Should I tag the Product Owner on delivery issues?**  
Only if the issue is related to priority conflicts or stakeholder decisions. Most blockers are resolved within the delivery team.

**Q: I’ve mentioned the same issue multiple times — nothing’s happened.**  
Escalate formally. Recurring blockers are a delivery risk. Bring it up again during Retrospective if still unresolved.

**Q: What if it’s sensitive or involves disagreement within the team?**  
Speak to the Scrum Master directly. They’ll help address the issue constructively and ensure it’s handled without blame.

---

Escalation keeps the team moving — not just informed.  
Raise early. Track clearly. Resolve together.
