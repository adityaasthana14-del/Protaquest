# 🧭 ProtaQuest

## The problem
Quitting a habit is hard, and most people do it alone. Existing habit-tracking apps only record streaks — they don't explain *why* day 3 feels worse than day 1, what the coming weeks will feel like, or what to do after a relapse. That missing guidance is where most people give up.

## The solution
ProtaQuest combines habit tracking with an AI guide that walks the journey with you.

- **Daily check-in:** log your mood and craving level; the AI guide explains why you feel this way at your stage and what the next few days usually look like.
- **"Craving now" support:** a 1-minute guided breathing exercise plus three immediate steps from the AI guide.
- **Guilt-free relapse flow:** log what triggered the slip; the guide helps you understand it and plan for next time. Your streak restarts, but your XP and history stay.
- **Journey map:** a Day 0–90 view of what most people go through at each stage, and where you are now.
- **Gamification:** XP, levels, daily side quests and a running total of money saved.
- **You vs. typical:** your average craving level compared with a typical pattern at your stage.
- **Guide chat:** talk to the AI guide anytime, in English or Hinglish.

## AI / ML used
- **Large Language Model (Anthropic Claude)** for personalised, context-aware guidance.
- **Prompt engineering with context injection:** each request includes the user's habit, their reason for quitting, current stage, streak, relapse count and recent check-ins.
- **Safety guardrails:** the guide recommends seeing a doctor for substance dependence and points to the Tele-MANAS helpline (14416) in a crisis.

> The AI guide runs in the claude.ai-hosted version. This standalone GitHub Pages version uses rule-based fallback guidance, so the full app flow still works without login.

## Tech stack
HTML, CSS, JavaScript (single-file, no build step). Data is stored locally in the browser.

## Roadmap
- [ ] FastAPI backend with PostgreSQL for user accounts and synced data
- [ ] LLM API integration so the AI guide works in the standalone version
- [ ] ML-based relapse-risk prediction from check-in history, to send proactive nudges before high-risk moments
- [ ] Mobile app with daily reminders
- [ ] Anonymous community milestones ("X people crossed day 7 today")

## Disclaimer
ProtaQuest is a pilot. It is not medical advice or a substitute for professional help.
