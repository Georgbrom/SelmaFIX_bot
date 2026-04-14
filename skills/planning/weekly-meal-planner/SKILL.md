Name: weekly-meal-planner

Purpose:
Plan a weekly menu and generate a shopping list every Sunday at 10:00, while minimizing food waste and API usage.

Trigger:
- Every Sunday at 10:00
- Or when the user asks for weekly meal planning

---

Behavior:

STEP 1 — Gather current inventory
- Ask the user:
 - What do you have in the fridge?
 - Are there any freezer items you want to use?
 - Any dry goods (rice, pasta, cans) you want to use up?

- Do NOT proceed until the user answers

---

STEP 2 — Understand constraints
- Identify:
 - Ingredients that should be used soon
 - User preferences (from memory if available)
 - Number of meals needed

- If needed:
 - Ask follow-up questions (keep it minimal)

---

STEP 3 — Check memory before searching
- Look for:
 - previously used meals
 - known preferences
 - saved recipes

- Prefer memory over web_search

---

STEP 4 — Use web_search (ONLY if needed)
- Only search if:
 - lacking recipe ideas
 - needing inspiration

- Limit:
 - maximum 1–2 searches

- Focus searches:
 - specific ingredients (e.g. "recipes with chicken and rice")

---

STEP 5 — Create weekly menu
- Generate a structured plan:
 - 5–7 meals
 - balanced and realistic
 - prioritize using existing ingredients

- Avoid:
 - overly complex meals
 - unnecessary new ingredients

---

STEP 6 — Generate shopping list
- Only include:
 - missing ingredients

- Organize by category:
 - vegetables
 - protein
 - dairy
 - dry goods

---

STEP 7 — Save useful information to memory
- Store:
 - successful meals
 - user preferences (likes/dislikes)
 - recurring ingredients

- Do NOT store:
 - full recipes
 - temporary plans

---

Rules:

- Minimize web_search usage
- Prefer existing ingredients over new purchases
- Keep plans simple and realistic
- Avoid unnecessary follow-up questions
- Always confirm unclear information before proceeding

---

Goal:
Reduce food waste, save money, and create a consistent, efficient weekly planning routine.