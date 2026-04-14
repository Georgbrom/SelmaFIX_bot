Name: skill-discovery

Purpose:
Continuously improve the agent by discovering, evaluating, and proposing new skills from ClawHub.

Trigger:
- Once daily
- Or when explicitly asked to find new skills

---

Behavior:

STEP 1 — Search for new skills
- Use web_search to find recent or relevant skills from ClawHub
- Focus on:
 - practical usefulness
 - simplicity
 - alignment with current system

- Limit:
 - maximum 1 search

---

STEP 2 — Select candidate
- Choose ONE skill that:
 - solves a real problem
 - improves efficiency
 - fits existing architecture

- Avoid:
 - overly complex skills
 - unsafe or unclear skills

---

STEP 3 — Analyze the skill
- Identify:
 - what it does
 - how it works
 - required tools
 - potential risks

---

STEP 4 — Adapt to system
- Suggest improvements:
 - simplify if needed
 - align with memory rules
 - align with existing skills

- Do NOT copy blindly

---

STEP 5 — Present proposal
Return:

1. Skill name
2. What problem it solves
3. Why it is useful
4. Suggested modifications
5. Recommendation (implement / skip)

---

STEP 6 — Wait for approval
- Do NOT implement automatically
- Ask user before adding any skill

---

Rules:

- Minimize web_search usage
- Prefer quality over quantity
- Never install or execute unknown skills automatically
- Always adapt skills to the existing system

---

Goal:
Gradually improve the agent without introducing instability or unnecessary complexity.