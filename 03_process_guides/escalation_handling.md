# 🚦 Escalation Handling

Escalation is not failure — it's how the team stays unblocked, aligned, and focused. This file defines when, how, and by whom issues should be escalated, both inside and outside the team.

> 📌 Escalation is a structured signal, not an emotional one. It's how the team protects momentum.

---

## 🎯 Purpose

- Ensure blockers are surfaced and resolved quickly
- Avoid misalignment between team roles or external stakeholders
- Create transparency around unresolved risks or delays
- Maintain delivery rhythm without individual burden

---

## 🧭 What Should Be Escalated?

| Escalation Type                   | Examples                                                                |
| --------------------------------- | ----------------------------------------------------------------------- |
| **Delivery Blockers**             | Unavailable inputs, permissions, credentials, data feeds                |
| **Planning Misalignment**         | Story too large for sprint, unclear Feature scope, overlap in ownership |
| **External Dependencies**         | Waiting on another team, system, vendor                                 |
| **Decision or Priority Conflict** | Competing stakeholder requests, unclear PO guidance                     |
| **Repeated Issues**               | Same blocker or bug showing up across sprints                           |

---

## 🧩 Escalation Flow

```
[Issue Detected]
↓
[Can I resolve this myself?] — Yes → [Resolve and move on]
↓ No
[Raise in Daily Standup]
↓
[Scrum Master triages issue]
↓
[Is this a delivery blocker?] — No → [Track and revisit later]
↓ Yes
[Scrum Master and Scope Lead coordinate resolution]
↓
[Escalate externally if needed → Scope Coordinator + PO]
```

---

## 🧑‍🤝‍🧑 Roles in Escalation

| Role                  | Responsibility                                           |
| --------------------- | -------------------------------------------------------- |
| **Product Developer** | Flags blockers early and clearly                         |
| **Scrum Master**      | Facilitates unblocking, triages risk level               |
| **Scope Lead**        | Resolves intra-sprint blockers or alignment issues       |
| **Scope Coordinator** | Escalates to external teams or PO if needed              |
| **Product Owner**     | Involved only in priority conflict or external decisions |

---

## ⏱️ Timing Guidelines

| Escalation Type           | Escalate Within          |
| ------------------------- | ------------------------ |
| Critical delivery blocker | 1 working day            |
| Repeated Story ambiguity  | Before next refinement   |
| Planning conflict         | Before next sprint cycle |
| External dependency delay | 48 hours (if no update)  |

---

## 🔄 Where to Track Escalated Issues

| Type                  | Tracking Location                                          |
| --------------------- | ---------------------------------------------------------- |
| Blocked Task or Story | Azure DevOps → move to `Blocked` column and add note       |
| Dependency or risk    | Backlog note + call out in Standup or Strategic Refinement |
| Cross-team issue      | Slack/Teams escalation + backlog tag (`external`)          |

---

## 🧠 Best Practices

- Escalate early — don’t wait for blockers to resolve themselves
- Keep language neutral and objective — focus on facts and impact
- Don’t escalate privately — blockers should be visible to the team
- Follow through — if you raise it, track it until it’s cleared

---

## ❓ FAQ

**Q: I’m blocked but unsure who can resolve it. What do I do?**  
A: Raise it in Standup. Scrum Master will triage or find the right person to help.

**Q: Should I tag the Product Owner on delivery issues?**  
A: Only if it’s a priority conflict or external alignment issue. Most delivery blockers are handled within the team.

**Q: I’ve raised the same issue multiple times. What next?**  
A: If it repeats across sprints, log it as a delivery risk. Scrum Master and Scope Lead will escalate to Scope Coordinator for systemic resolution.

**Q: What if it’s sensitive or involves disagreement?**  
A: Raise it with the Scrum Master privately first, but it must still be tracked transparently in some form.

---

Escalation is how teams stay aligned and accountable — not how blame is assigned.  
Raise early. Track clearly. Resolve together.
