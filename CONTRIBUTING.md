# Contributing to Business Prompts

Thank you for helping build the world's best open-source business prompt library.

This guide covers everything you need to know to contribute a high-quality prompt that gets merged.

---

## What We're Looking For

Every prompt in this library is **production-ready** — meaning it consistently produces professional-quality output that a business operator could use immediately. We are not a collection of prompt experiments or AI novelties.

**A great contribution:**
- Solves a real, recurring business task
- Uses the WEDGE Framework (see below)
- Produces output a professional wouldn't be embarrassed to send
- Works across at least 2 major AI tools (ChatGPT, Claude, Gemini, etc.)
- Has been tested by the contributor with real input

**We don't accept:**
- Generic prompts ("write a business email")
- Prompts that require niche tools or proprietary context
- Duplicate prompts that closely resemble existing entries
- Prompts without `[bracketed placeholders]`
- Untested prompts

---

## The WEDGE Framework

All prompts in this library follow the **WEDGE Framework**, developed by [WEDGE Method LLC](https://thewedgemethodai.com):

| Element | Description | In Prompt |
|---------|-------------|-----------|
| **W** — Who | Sets the AI's role and expertise | `You are a [expert role]...` |
| **E** — Establish Context | Provides background the AI needs | `**Context:** ...` section |
| **D** — Define Deliverable | Specifies exactly what to produce | `**Deliverable:** ...` section |
| **G** — Guide Constraints | Sets quality and format standards | `**Constraints:** ...` section |
| **E** — Evaluate | Builds in a self-check | `**Before responding, evaluate:** ...` line |

Every contributed prompt must include all five elements.

---

## Prompt Template

Copy this template when writing a new prompt:

```markdown
### [Prompt Name]

**Use when:** [One sentence describing when to use this prompt]

**Prompt:**

> You are [specific expert role with relevant background]. [Optional: brief statement of expertise].
>
> I need you to [task description].
>
> **Context:**
> - [Field 1]: [placeholder description]
> - [Field 2]: [placeholder description]
> - [Field 3]: [placeholder description]
> (add as many as needed — aim for 5–10 context fields)
>
> **Deliverable:**
> [Clear, specific description of exactly what the AI should produce. Format, length, structure.]
>
> **Constraints:**
> - [Specific quality guideline 1]
> - [Specific quality guideline 2]
> - [Format requirement]
> - [Tone or style requirement]
> (3–6 constraints)
>
> **Before responding, evaluate:** [One question the AI should ask itself before answering — ensures quality over speed]

**Example output preview:** [Optional but encouraged — 2–4 lines showing what a good response looks like]

---
```

---

## Placeholder Format

Use square brackets for all user-filled fields:

| Format | Use for |
|--------|---------|
| `[Your Name]` | Clear single value |
| `[Company Name]` | Business or entity name |
| `[Description]` | Paragraph or multi-sentence input |
| `[Optional: description]` | Fields the user may skip |
| `[e.g., 30 / 45 / 60 minutes]` | Field with example options |

Do NOT use angle brackets (`<like this>`) or ALL_CAPS (`LIKE_THIS`). Square brackets are the standard.

---

## Quality Standards

Before submitting, verify your prompt meets these criteria:

### Completeness
- [ ] Includes all five WEDGE elements (Who, Establish Context, Define Deliverable, Guide Constraints, Evaluate)
- [ ] Has a clear "Use when" description
- [ ] Has 5–10 context fields with meaningful `[placeholders]`

### Testability
- [ ] You have personally run this prompt with real input
- [ ] The output was genuinely useful without heavy editing
- [ ] The prompt works in at least two AI tools

### Quality bar
- [ ] Output could be used professionally without significant revision
- [ ] Constraints are specific, not generic ("avoid jargon" is fine; "be professional" is too vague)
- [ ] "Before responding, evaluate" question meaningfully improves the output quality

### Formatting
- [ ] Follows the exact template above (blockquote format for prompt body)
- [ ] Has a `---` separator at the end
- [ ] Fits cleanly into an existing category or includes a clear case for a new one

---

## Adding to an Existing Category

If your prompt fits an existing category:

1. Fork the repository
2. Edit `README.md`
3. Find the appropriate category section
4. Add your prompt at the end of that category section, following the template
5. Update the category count in the section header if needed
6. Submit a pull request

---

## Proposing a New Category

Before creating a new category, check that:
- The category doesn't exist already (including as a section within an existing category)
- The category has at least 8 prompts ready to fill it (stub categories aren't useful)
- The category represents a real, recurring business function

To propose a new category:
1. Open an issue titled: `[New Category] [Category Name]`
2. List 8+ prompt titles you plan to contribute
3. Wait for maintainer approval before submitting the PR

---

## Editing Existing Prompts

If you find an existing prompt that:
- Produces low-quality output
- Has a broken structure
- Misses an important context field
- Has an inaccurate "Use when" description

Open an issue or submit a PR with your improvement. Explain what changed and why in the PR description.

---

## Pull Request Process

1. Fork the repo and create a branch: `prompt/[category]-[prompt-name]`
   - Example: `prompt/sales-cold-email-follow-up-v2`
2. Make your changes
3. Test the prompt with real input (include a brief note in the PR about what you tested)
4. Submit the PR with:
   - What you added or changed
   - Why it belongs here
   - Brief testing notes

---

## Code of Conduct

This is a professional resource. All contributions should:
- Be appropriate for a business context
- Be respectful to all contributors and users
- Not include prompts designed to manipulate, deceive, or harm

---

## Questions?

Open an issue or reach out at [thewedgemethodai.com](https://thewedgemethodai.com).

---

*Built on the [WEDGE Framework](https://thewedgemethodai.com) by WEDGE Method LLC.*
