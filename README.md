# TS Digital DM Engine

An AI-powered lead generation and outreach engine that turns hours of manual prospecting into a single automated flow.

**Live demo:** [ts-digital-dm-engine.vercel.app](https://ts-digital-dm-engine.vercel.app)

---

## The Problem

While running client-facing work, I hit the same bottleneck every single day: finding the right industry-specific prospects and writing a personalised outreach message for each one was slow, repetitive, and impossible to scale. Every new lead meant researching the business, understanding their context, and manually crafting a message that didn't sound like a template. Hours went into work that produced a handful of DMs.

I didn't want a bigger to-do list. I wanted the problem to go away.

## The Solution

So I built one. The DM Engine lets you:

1. **Search** for prospects by industry and niche
2. **Qualify** them automatically against relevant criteria
3. **Generate** a tailored, human-sounding outreach DM for each prospect using AI

What used to take hours of manual research and writing now runs as a single flow. The engine handles the repetitive work; the human stays in control of the final send.

## How It Works

The engine uses the Claude API as its core reasoning layer. When a user searches for a given industry, the backend gathers relevant prospect context, applies qualification logic, and prompts the model to craft an outreach message personalised to that specific prospect — not a generic template.

The prompt design went through multiple iterations. I tested different prompt structures and messaging approaches, kept what produced the highest-quality, most natural output, and discarded what didn't. That iteration is where most of the real work happened.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS |
| Backend | Node.js |
| AI / Reasoning | Claude API |
| Deployment | Vercel |

## Project Structure

```
ts-digital-dm-engine/
├── api/
│   └── scout.js        # Core backend logic — prospect search, qualification, DM generation
├── index.html          # Frontend interface
└── README.md
```

## Running Locally

```bash
# Clone the repository
git clone https://github.com/tsdigital-tushar/ts-digital-dm-engine.git
cd ts-digital-dm-engine

# Add your Claude API key to environment variables
# (create a .env file — do not commit it)
ANTHROPIC_API_KEY=your_key_here

# Install dependencies and run
npm install
npm start
```

## Why I Built This

I'm a builder before I'm anything else. When I see a repetitive problem, my instinct is to design a system that removes it rather than grind through it manually. This project is a small proof of that instinct: spot the bottleneck, define the solution as a product, build it, ship it live.

---

*Built by Tushar Singh.*
