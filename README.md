# Creative Prompting Skill

A Claude Code skill that enhances creative outputs by generating diverse candidates and selecting the best one, based on Stanford NLP research.

## What This Does

This skill helps Claude break free from predictable, "safe" responses by tapping into the full range of its creative capabilities. When you ask for something creative, unique, or original, this skill generates multiple diverse candidates internally and selects the best one instead of defaulting to the most conventional response.

## When to Use

Use this skill when you want:
- **Creative writing** (stories, poems, jokes, taglines, scripts)
- **Naming and branding** (product names, company names, slogans)
- **Brainstorming and ideation**
- **Original marketing copy and hooks**
- **Dialogue and character voices**
- **Anything that shouldn't sound like "typical AI output"**

## How to Trigger

Use phrases like:
- "give me something creative"
- "make it unique"
- "surprise me"
- "think outside the box"
- "be original"
- "I want something unexpected"

## The Science Behind It

Research from Stanford NLP found that during RLHF training, human raters consistently scored predictable, safe answers higher. This taught models to suppress their most interesting and diverse ideas. The diversity was never deleted—just buried beneath risk-averse optimization.

This skill recovers that hidden diversity by generating multiple candidates from the full output distribution, then selecting the best one. Studies show this can produce:
- **2x more diverse** creative writing
- **More natural** dialogue patterns
- **18% better accuracy** in synthetic data tasks

## Installation

1. Copy `SKILL.md` to your Claude Code skills directory
2. The skill will be automatically available in Claude Code

## How It Works

When triggered, the skill:

1. **Reframes** the task from multiple creative angles
2. **Generates** 5 diverse candidates across the spectrum from conventional to unexpected
3. **Selects** the best one based on originality, quality, and fit
4. **Delivers** the refined result naturally (the process is invisible unless you ask for multiple options)

## Example

Instead of getting a conventional response like "Here are some marketing ideas...", you might get something truly creative and unexpected that still perfectly serves your needs.

---

*This skill is designed to work with Claude Code's skill system. For more information about creating skills, see the Claude Code documentation.*