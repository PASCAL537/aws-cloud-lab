# AWS Cloud Lab — 100 Days of Cloud Challenge

> Hands-on AWS and Azure labs completed as part of the **#100DaysOfCloudLabs** challenge on KodeKloud.
> Each entry documents what was done, the concept behind it, and how it applies to real-world cloud infrastructure.

---

## Lab Progress

| Cloud | Days Completed |
|---|---|
| AWS | 19+ days |
| Azure | 24+ days |

---

## Day 19 — IAM: Attaching a Policy to a User

**Platform:** AWS (KodeKloud)
**Topic:** Identity and Access Management (IAM)
**Difficulty:** Foundational
**Time:** Short lab — but the concept is critical

### What I Did

Attached an IAM policy to an existing IAM user.

**Starting state:**
- User `iamuser_mariyam` existed ✅
- Policy `iampolicy_mariyam` existed ✅
- But they were not connected ❌ — the user had zero access

**Action taken:**
- Navigated to IAM in the AWS Console
- Located the user and attached the policy directly

**Result:**
- User now has exactly the permissions defined in the policy — nothing more, nothing less

### The Concept: Why This Matters

Without a policy attached, an IAM user is just an empty identity — an ID card with no doors to open.

Attaching the policy is what activates access. And because IAM policies define permissions explicitly, there is no guessing, no over-privilege, no shared credentials.

### Real-World Application

This is how access control works at scale in real companies:

1. New engineer joins → IAM user created
2. Their role is defined → policy created or selected
3. Policy attached to user → they get exactly what they need
4. They leave → policy detached → access revoked instantly

No shared passwords. No over-privileged accounts. Clean, controlled, auditable access.

### Key Takeaway

> IAM is not just a setup step — it is the security backbone of every AWS environment.
> The principle of **least privilege** (give users only what they need) starts here.

### Tags
`AWS` `IAM` `Cloud Security` `Least Privilege` `Access Control` `KodeKloud` `100DaysOfCloud`

---

*More labs being added as the challenge progresses. Follow along on [LinkedIn](https://www.linkedin.com/in/ifeanyi-pascal-okonkwo-6b22b1128)*
