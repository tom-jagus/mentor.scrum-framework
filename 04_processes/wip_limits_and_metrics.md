# 📊 WIP Limits & Delivery Metrics

WIP limits and delivery metrics help the team maintain focus, reduce overload, and measure delivery health over time. They are not performance tools — they are signals used to protect flow and guide improvement.

---

## 🎯 Purpose

- Prevent overcommitment and context switching
- Surface delivery risks early
- Create visibility into how work is flowing (or not)
- Support retrospectives, planning, and decision-making with real data

---

## 🔧 WIP Limits

**WIP** (Work in Progress) is anything that has started but isn’t finished.  
The more WIP we carry, the more risk we introduce — to focus, quality, and outcomes.

---

### 🛑 Default WIP Limits

| Scope         | Limit                                     |
| ------------- | ----------------------------------------- |
| Per Developer | Max **2** Stories `In Progress`           |
| Per Story     | Max **5** open Tasks                      |
| Per Sprint    | Max **80%** of capacity committed upfront |

> These are guidelines, not hard stops — but exceeding them requires a conversation.

---

### ✅ WIP Enforcement Rules

- Developers may not start more than 2 Stories without completing others
- Tasks should be pulled one at a time — finish, then start
- Scrum Master monitors board for WIP drift during Standup
- Excess WIP is reviewed in Retrospective

---

### 🚫 WIP Anti-Patterns

- Multiple Stories or Tasks started with none moving forward
- Stories left half-done at sprint close
- WIP limits ignored in favor of “feeling busy”
- Stories dragged across multiple sprints

---

## 📈 Delivery Metrics

Delivery metrics help the team reflect on throughput, quality, and work type balance. They are reviewed regularly — not daily — and used in Review, Retro, and roadmap decisions.

---

### 📊 Core Metrics

| Metric              | What It Measures                                    | Why It Matters                            |
| ------------------- | --------------------------------------------------- | ----------------------------------------- |
| **Velocity**        | Number of completed Story Points per sprint         | Tracks sustainable pace over time         |
| **Cycle Time**      | Time from `In Progress` → `Done` (per Story)        | Highlights bottlenecks in delivery        |
| **Carryover Rate**  | % of Stories not completed in the sprint            | Signals overcommitment or poor refinement |
| **Work Type Ratio** | % split between Project, Support, Maintenance, Bugs | Ensures delivery balance and visibility   |

---

### 📆 How We Use Metrics

- Velocity trends are reviewed every 3–4 sprints
- Carryover rate is discussed during Retrospective
- Cycle time outliers trigger investigation by the Scrum Master
- Work type mix is reviewed monthly to ensure team health

---

## 🧠 Best Practices

- Keep WIP visible and updated — don’t “mentally” track your work
- Treat metrics as feedback, not evaluation
- Look for patterns across multiple sprints — not single-point anomalies
- If metrics feel off, dig into process — not people

---

## ❓ FAQ

**Q: Can I ignore WIP limits if I feel productive?**  
No. WIP limits are about system flow, not individual pace. Too much WIP slows everyone down.

**Q: What if my Story requires many Tasks?**  
Break it into smaller Stories, or ensure the Tasks are logically grouped. Overloaded Stories often signal poor refinement.

**Q: What if velocity drops suddenly?**  
Check refinement quality, unplanned work, or blocker trends. Don’t jump to conclusions — investigate the system.

**Q: How do we handle spikes or exploratory work in metrics?**  
Track them with timebox tags or separate swimlanes. They count as work — but we don’t estimate them like Stories.

**Q: What’s an acceptable carryover rate?**  
Occasional carryover is fine — especially for legitimate blockers. Consistent carryover means refinement or planning needs attention.

---

Limits protect the flow.  
Metrics reveal the truth.  
Together, they help the team deliver intentionally — and improve with confidence.
