---
name: creative-prompting
description: >
  Enhance creative outputs by generating diverse candidates and selecting the best one.
  Use this skill when the user explicitly asks for creative, diverse, unique, original,
  or unexpected outputs — e.g., "give me something creative," "make it unique,"
  "surprise me," "think outside the box," "be original,"

---

# Creative Prompting

## Background

Research from Stanford NLP found that LLMs have been inadvertently trained to suppress their most interesting and diverse ideas. During RLHF, human raters consistently scored predictable, safe answers higher — so models learned to play it safe. The diversity was never deleted from the model's knowledge, just buried beneath layers of risk-averse optimization.

A simple technique recovers this hidden diversity: instead of generating one response directly, generate multiple candidates sampled from the full output distribution, then select the best one. This has been shown to produce up to 2x more diverse creative writing, dialogue that's closer to real human conversational patterns, and 18% better downstream accuracy in synthetic data generation tasks.

## How This Skill Works

When the user asks for creative, diverse, or original output, follow this process instead of responding directly. The goal is to tap into the full range of what you actually know how to produce, rather than defaulting to the safest option.

### Step 1: Reframe the task internally

Before generating anything, think about the user's request from multiple angles. Consider:

- What are 3-5 genuinely different *approaches* to this task? Not variations on one approach — structurally different takes.
- What would a surprising but good response look like?
- What's the "obvious" response you'd normally give? Deliberately set that aside.

### Step 2: Generate 5 diverse candidates

Generate 5 responses to the user's request. These should be sampled from across the full distribution of reasonable responses — not 5 slight variations of the same idea. Each candidate should take a meaningfully different angle, tone, structure, or creative direction.

Think of it this way: if you lined up all possible good responses to this prompt from most conventional to most unexpected, your 5 candidates should be spread across that spectrum, not clustered at the "safe" end.

For each candidate, briefly note (to yourself) what makes it distinct from the others.

### Step 3: Select and refine

Pick the single best candidate based on:

1. **Originality** — Does it avoid the predictable, default response?
2. **Quality** — Is it well-crafted regardless of its unconventionality?
3. **Fit** — Does it actually accomplish what the user asked for?

If the best candidate is great but could be refined, humanize it. Then deliver that single response to the user as your answer. Don't show the user all 5 candidates or mention this process unless they ask for multiple options.

### When the user asks for multiple options

If the user explicitly wants several options to choose from (e.g., "give me a few ideas," "show me some options"), present 3-5 of the candidates directly, ordered from most conventional to most unexpected. Let the user know which one you'd recommend and why.

## What This Applies To

This technique works across any task where diversity and originality matter:

- Creative writing (stories, poems, jokes, taglines, scripts)
- Naming and branding (product names, company names, slogans)
- Brainstorming and ideation
- Dialogue and character voice
- Marketing copy and hooks
- Synthetic data generation
- Any request where the user signals they want something that doesn't sound like "typical AI output"

## What to Avoid

- Don't sacrifice quality for novelty. An original but bad response is worse than a conventional but good one. The goal is to find the response that's *both* original and high-quality.
- Don't make the process visible to the user unless they ask. Just deliver the best response naturally.
- Don't apply this technique to factual, technical, or precision-oriented tasks where there's a correct answer. This is for tasks with a wide space of valid creative responses.