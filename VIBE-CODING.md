# TradeMind – Vibe Coding Documentation

## Overview

TradeMind is a trade journaling and reflection tool designed for beginner traders.

It helps users:
- reflect on past trades
- identify behavioural patterns
- receive AI-generated insights
- improve their next decisions

This project was built using AI as a co-pilot throughout ideation, UX design, development, and troubleshooting.

## Approach

Instead of writing everything manually, I used AI as a co-pilot to:

- define the product concept
- design the user experience
- generate UI code
- integrate AI-powered insights
- debug issues and refine the app

My role focused on UX writing and product thinking, while AI helped accelerate implementation.

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
"Build a clean web app using HTML, Tailwind CSS, and JavaScript based on this structure..."

Outcome:
Generated the initial UI layout for all three screens.

---

### Prompt 2: AI Insight Logic
"Analyse this beginner trader's reflection and return pattern, mistake, and next step..."

Outcome:
Created structured, beginner-friendly insights.

---

### Prompt 3: Refining UX Copy
"Rewrite this UI copy to be clearer, more supportive, and beginner-friendly..."

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
