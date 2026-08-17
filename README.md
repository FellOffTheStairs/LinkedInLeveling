# Visibility Roadmap Game

A gamified career roadmap: audit your LinkedIn profile, compare yourself to the market average for your target role, turn the gaps into a roadmap, then turn the roadmap into a playable RPG with turn-based battles.

**[Live demo](#)** ← replace with your GitHub Pages link once deployed

This repo comes preloaded with an **AI Engineer** version as an example. To build your own version for a different role, follow the prompt guide below with your AI assistant of choice (Claude, ChatGPT, etc.) — you're not editing code by hand, you're having a conversation and letting the assistant generate a new HTML file for you.

---

## How to build your own version

Copy each prompt below into your AI assistant, one at a time, filling in the blanks. Do them in order — each step builds on the last.

### Step 1 — Audit your profile
> "Here's my LinkedIn profile: [paste your profile URL or paste your headline/About/Experience sections]. I'm aspiring to become a **[YOUR TARGET ROLE, e.g. Product Manager, Data Analyst, UX Designer]**. Critique it honestly — what's missing, what's weak, and what a recruiter would flag."

*If your assistant has a LinkedIn tool/plugin connected, ask it to pull your profile directly instead of pasting.*

### Step 2 — Compare to the market average
> "Now compare my profile against what a strong, market-average **[YOUR TARGET ROLE]** candidate looks like today — skills, project types, proof of work, keywords, portfolio. What's the gap between where I am and where I need to be?"

### Step 3 — Turn the gap into a roadmap
> "Turn everything that's missing into a step-by-step roadmap I can work through, broken into chapters (e.g. Profile, Projects, Posts, Proof, Skills, Portfolio — adjust chapter names to fit **[YOUR TARGET ROLE]**). Each chapter should have concrete, checkable tasks."

### Step 4 — Translate the roadmap into RPG equipment
> "Now translate those roadmap chapters into RPG equipment. Keep the chapter names. Each chapter earns a piece of equipment (give them names that fit a **[YOUR TARGET ROLE]** theme), each with 3 levels of perks, plus a stat system that reflects what actually matters for **[YOUR TARGET ROLE]** (e.g. Signal, Craft, Proof, Systems — adjust to fit). Suggest a player class name too."

### Step 5 — Build it into a playable dashboard
> "Build this into a single HTML file: a dashboard with three tabs — Quests (the real roadmap tasks, checkable), Armory (the RPG equipment and stats, leveling up as I complete quests), and Play (a Pokémon-style turn-based battle screen where my stats come from my real progress). Use a dark sci-fi theme, keep it all in one HTML file, and save my progress in the browser (localStorage) so it persists."

### Step 6 (optional) — Polish
> "Add pixelated humanoid avatars for the battle screen — blue for me, red for the enemy." <br>
> "For every equipment level, show the exact stat boost it gives before I unlock it, so there's anticipation for what's coming."

---

## Deploying your version

1. Fork this repo (or create a new one).
2. Replace `ai-engineer-roadmap.html` with your generated file (rename it to something like `your-role-roadmap.html`, or keep it as `index.html` if you want it to load automatically).
3. In your repo: **Settings → Pages → Deploy from branch → main → / (root)**.
4. GitHub gives you a live URL at `https://<your-username>.github.io/<repo-name>/` — share that link with anyone.
5. Update the demo link at the top of this README.

Progress is saved per-browser via `localStorage`, so each visitor's save state is their own — no backend or database needed.

---

## Notes

- This is a static, single-file HTML app — no build step, no server required.
- Want to support multiple roles in one deployed site (e.g. a dropdown to pick "AI Engineer" vs "Product Manager")? That's a bigger lift — worth a separate build once you've got a couple of role-specific versions made this way and want to merge them.
