# 🐞 Bug Handling

Bugs are not second-class work. They are tracked, validated, prioritized, and delivered with the same rigor as User Stories — using defined lifecycles, roles, and visibility rules.

This process ensures that issues are not hidden, misprioritized, or handled inconsistently. Bugs are work — and they move through the same delivery system.

---

## 🎯 Purpose

- Ensure Bugs are handled transparently and consistently
- Clarify how Bugs are validated, prioritized, and resolved
- Define roles and expectations across triage, development, and verification
- Maintain quality and delivery standards without disruption

---

## 🐛 What Counts as a Bug?

A **Bug** is any functional issue that meets **all three** of the following:

- The system does not behave as expected
- The deviation is not part of a scope change
- The issue is reproducible or observable in a specific context

Bugs include logic errors, UI defects, missing behavior, data issues, or failure to meet acceptance criteria after release.

---

## 🔁 Status Lifecycle

| Status        | Description                                               |
| ------------- | --------------------------------------------------------- |
| `New`         | Reported and pending triage                               |
| `Confirmed`   | Reproducible and accepted for resolution                  |
| `In Progress` | Assigned Developer is working on a fix                    |
| `In Review`   | Fix complete — pending validation by Analyst or peer      |
| `Resolved`    | Bug confirmed fixed and validated in expected environment |

---

## 👥 Roles & Responsibilities

| Role                  | Responsibility                                           |
| --------------------- | -------------------------------------------------------- |
| **Reporter**          | Logs the Bug with full reproduction details              |
| **Product Analyst**   | Validates and confirms that the issue qualifies as a Bug |
| **Product Developer** | Fixes the Bug and ensures technical quality              |
| **Scrum Master**      | Ensures Bugs are visible and prioritized properly        |

---

## ✅ Triage Criteria

Bugs must be confirmed before being worked on. A Bug is **Confirmed** when:

- [ ] Expected vs. actual behavior is clearly described
- [ ] The issue is reproducible (or well-documented if environment-specific)
- [ ] Impact is understood (severity, scope, frequency)
- [ ] Analyst agrees that it is not scope drift or enhancement
- [ ] Linked to affected Story, Feature, or Epic (if applicable)

---

## 🧪 Validation Checklist

A Bug may be marked **Resolved** when:

- [ ] The issue no longer occurs
- [ ] Fix was validated by an Analyst or peer Developer
- [ ] A regression case was considered or documented
- [ ] Status is updated and fix is linked to board item or PR

---

## 🔄 Prioritization & Planning

| Bug Type             | Action                                                                  |
| -------------------- | ----------------------------------------------------------------------- |
| **Blocking Bug**     | Escalated immediately. May interrupt sprint scope if affecting delivery |
| **Major Bug**        | Added to next sprint. Prioritized alongside Stories                     |
| **Low Priority Bug** | Added to triage list or support backlog. Reviewed weekly                |

Bugs must never be silently fixed. All work, even “quick fixes,” must be tracked and validated.

---

## 📊 Visibility

- Bugs appear on the Scrum board just like Stories
- Severity or impact may be indicated with tags, labels, or priority flags
- Repeat Bugs are discussed during Retrospective to identify patterns or gaps
- All Bugs are included in Review if resolved during the sprint

---

## 🚫 Anti-Patterns

- Fixing a Bug without tracking it
- Closing Bugs without independent validation
- Labeling edge cases or poor design as “not a bug” without Analyst input
- Ignoring repeat Bugs without root cause follow-up

---

## ❓ FAQ

**Q: Can I fix a Bug without filing it first?**  
No. All work must be tracked. Even quick fixes need a Bug record for validation and historical visibility.

**Q: Who decides if something is really a Bug?**  
The Product Analyst confirms whether an issue qualifies as a Bug or scope clarification.

**Q: Can Bugs interrupt the sprint?**  
Only if they are blocking delivery. All others are reviewed and scheduled just like Stories.

**Q: How do we handle UI/UX Bugs discovered post-release?**  
If they violate intended behavior, treat them like any Bug. If they relate to subjective polish, escalate to PO for product-level prioritization.

---

Bugs are not noise — they are signals.  
Handled with structure, they protect velocity and build trust.
