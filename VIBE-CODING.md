# TradeMind – Vibe coding documentation

## Overview

TradeMind is a trade journaling and reflection tool designed for beginner traders.

It helps users:
- reflect on past trades
- identify behavioural patterns
- receive AI-generated insights
- improve their next decisions

This project was built using AI as a co-pilot throughout ideation, UX design, development, and troubleshooting. AI tools include **ChatGPT** for brainstorming, **Claude** for high-level thinking and strategy, and **Google AI Studio** for app-building.

## Approach

I used a multi-AI workflow, treating different models as specialised collaborators across different stages of the build.

### 1. ChatGPT — Ideation & Structuring
ChatGPT was used early to:
- brainstorm product directions suitable for the hackathon
- refine the core problem and target user
- structure the initial product definition and MVP scope

This helped quickly move from a broad idea to a focused, buildable concept.

---

### 2. Claude — Product Thinking & UX Strategy
Claude was used for higher-level reasoning and product decisions, including:
- refining the user journey (Overview → Reflection → Insights)
- simplifying the feature set to avoid overbuilding
- shaping the UX writing principles (clear, calm, supportive)
- ensuring the product stayed focused on behaviour and decision-making rather than raw trading data

This step was critical in turning the app into a **thinking tool**, not just a logging tool.

---

### 3. Google AI Studio (Gemini) — Implementation & App Building
Google AI Studio was used as the primary development environment to:
- generate the initial UI using HTML, Tailwind CSS, and JavaScript
- implement the three core screens based on structured wireframes
- integrate the Gemini API for real-time insight generation
- iterate quickly on layout, functionality, and interaction logic

This enabled rapid prototyping without needing deep frontend framework knowledge.

---

### Overall Workflow
The development process followed a layered approach:

1. Define the problem and concept (ChatGPT)
2. Refine UX and product decisions (Claude)
3. Build and iterate the app (Gemini)

This combination allowed me to balance:
- speed (AI-generated code)
- clarity (UX and content design)
- focus (tight MVP and user flow)

## Key Product Decisions

### 1. Focus on reflection, not trading execution
Instead of building a full trading platform, I focused on helping users learn from past trades.

### 2. Simplify for beginner traders
All terminology and insights were written in plain English to avoid overwhelming users.

### 3. Structure the experience into 3 steps
- Overview → Reflection → Insights

This made the product easy to understand and use.

### 4. Emphasise actionable insights
The app does not just show data — it tells users what to improve next.

## How AI Was Used

AI was used in multiple stages of development:

### 1. Ideation
AI helped generate and refine product ideas suitable for a small team and hackathon constraints.

### 2. UX and Content Design
AI assisted in:
- structuring user flows
- refining microcopy
- improving clarity and tone

### 3. UI Development
AI generated the initial HTML, Tailwind, and JavaScript structure based on wireframes.

### 4. AI Insight Feature
The Gemini API was integrated to:
- analyse user reflections
- generate behavioural insights
- suggest next actions

### 5. Debugging
AI helped identify and fix issues such as:
- API integration errors
- UI rendering issues
- event handling bugs

## Key Prompts

### Prompt 1: Generating UI
"Objective: Build a polished, modern Single Page Application (SPA) for a trading journal called "TradeMind".
Brand Identity:
Tone: Professional, calming, and data-driven (SaaS/Fintech aesthetic).
Colors: Indigo/Purple primary, Slate/Neutral backgrounds, Emerald for wins, Rose for losses, and Amber for insights.
Typography: Inter (Sans-serif) with high-contrast headings.
Core Screens/Sections:
Overview Dashboard:
Navigation bar with a brand logo and section links.
Summary cards for Total P&L, Trades Count, and Win Rate.
A "Current Streak" card with a progress visual.
A "What stands out" callout for AI-generated patterns.
A "Trading Behavior" grid highlighting mistakes and strengths.
Trade Reflection:
A summary of the selected trade (Market, Entry/Exit, Outcome).
A multi-step form asking for: Entry Reason, Signal relied on, and "What to do differently next time".
An AI Insight box that appears after submission.
Insights & Learning:
A "Weekly Edge" section that stays locked behind a 7-day streak goal.
Segmented progress bar showing streak progress.
Grids for behavior patterns and common mistakes.
Settings:
Configuration for External API (Deriv) integration.
Data management options (Clear History).
Technical Requirements:
Use Tailwind CSS for all styling.
Use Lucide-React style icons.
Ensure a Mobile-First responsive layout (44px touch targets).
Implement smooth transitions between sections.
Use localStorage for data persistence."

Outcome:
Generated the initial UI layout for all three screens.

---

### Prompt 2: AI Insight Logic
"The "Trade Coach" Insight Prompt
Role: Trading Psychology Expert & Mentor
Task: Analyze a beginner trader's reflection.
Prompt Template:
Analyse this beginner trader's reflection. Identify:
the likely behaviour pattern,
the possible mistake,
one practical next step.
Instructions:
Keep the response supportive, concise, and in plain English.
Return the answer in exactly this format:
Pattern noticed: [Brief observation of their psychological or technical habit]
Possible mistake: [Specific error made in this trade]
Next step: [One actionable piece of advice for the next trade]
Context:
Reason for entering: {user_entry_logic}
Followed a clear plan: {yes_no}
Signal relied on: {indicator_or_price_action}
What to do differently next time: {user_self_reflection}"

Outcome:
Created structured, beginner-friendly insights.

---

### Prompt 3: Refining UX Copy
""

Outcome:
Improved readability and tone consistency across the app.

## Iteration Process

The app went through multiple iterations:

### Iteration 1
Basic UI structure with static content.

### Iteration 2
Added reflection form and simulated insights.

### Iteration 3
Integrated Gemini API for real-time insights.

### Iteration 4
Improved UX copy, layout clarity, and user flow.

Each iteration was guided by AI suggestions and manual refinement.

## Challenges & Troubleshooting

### Challenge 1: API Integration
Issue:
Difficulty integrating Gemini API into a frontend-only app.

Solution:
Used a simplified client-side fetch approach and added fallback handling.

---

### Challenge 2: Overcomplicated UI
Issue:
Initial design included too many metrics and overwhelmed the user.

Solution:
Simplified the UI to focus on key insights and actions.

---

### Challenge 3: Authentication with Deriv
Issue:
Full login integration added unnecessary complexity.

Solution:
Switched to demo mode to ensure the app remained functional and focused on its core purpose.

## AI vs Human Contribution

### What AI did well
- generated UI scaffolding quickly
- suggested code structures
- accelerated debugging

### What required human judgement
- defining the right product scope
- simplifying the UX for beginners
- crafting clear and supportive copy
- deciding what features to include or remove

## Future Improvements

- full integration with Deriv API for live trade data
- secure backend for API key handling
- personalised insights based on trade history
- richer analytics and visualisations
