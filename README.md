# product-discovery

A skill for Claude that works as a practical manual for product discovery: learning what is worth building before you build it. It covers the full cycle, from setting an outcome to interviewing customers, mapping opportunities, testing assumptions and sharing evidence with stakeholders.

Its fastest use is preparing customer conversations. Describe the project and who you will talk to, and it returns a ready-to-use interview guide.

## What it does

- **Prepares interview guides.** For a new project it first asks a few short questions (each with a default), then writes a timed guide with learning goals, beliefs to challenge, story-based questions with follow-ups, reminders for the interviewer and an after-meeting checklist.
- **Guides the whole discovery cycle.** Outcomes and learning goals, weekly interviews, opportunity solution trees, idea generation, assumption mapping, test design, decisions and stakeholder updates.
- **Produces usable artifacts.** Interview guides, interview snapshots, opportunity entries, assumption tables, test plans and stakeholder updates, using the templates in `references/templates.md`.
- **Corrects common mistakes** (asking customers what to build, hypothetical questions, tests with no success criteria) and says how strong the evidence really is.
- **Replies in your language.** Guides are written in the language of the request.

## Usage

Invoke it by name and describe what you need:

```
/product-discovery help me prepare a first meeting with a customer who is a personal trainer for older adults
```

For a new project, Claude replies first with a few questions, for example:

1. What are you exploring, and what decision will these conversations feed?
2. Who is the participant, and how do they relate to your target customer?
3. What do you already know?
4. What do you most want to learn from this meeting?

Answer briefly, or reply "defaults" to accept the assumptions it proposes. Claude then writes the complete guide. If you want a draft immediately, say so and it skips the questions.

Other requests that trigger the skill:

- "Turn these five interview notes into an opportunity solution tree."
- "List the riskiest assumptions behind this idea and design a cheap test for each."
- "Write a one-page update for my stakeholders on what we learned."
- "Review this interview script and tell me what is wrong with it."

It also triggers when you describe a discovery problem without using the word, such as validating an idea or deciding what to build next.

## Installation

**Claude (claude.ai or desktop app):** open Settings, go to Capabilities, then Skills, and upload `product-discovery.skill` (or a zip of the `product-discovery` folder).

**Claude Code:** copy the folder into your skills directory.

```bash
# for all projects
cp -r product-discovery ~/.claude/skills/

# or for one project
cp -r product-discovery <your-project>/.claude/skills/
```

Then start a new session and invoke `/product-discovery`.

## Structure

```
product-discovery/
├── SKILL.md                         Principles, 8-step workflow, fast path for interview guides
└── references/
    ├── interview-guide-builder.md   How to turn a short request into a full guide
    ├── example-interview-guide.md   A model: context questions plus finished guide
    ├── framing.md                   Outcomes, learning goals, experience maps, segments
    ├── interviewing.md              Cadence, recruiting, question bank, bad data, snapshots
    ├── opportunities-and-ideas.md   Opportunity solution trees, prioritizing, ideation
    ├── assumptions-and-testing.md   Assumption types, test design, test ladder
    ├── stakeholders-and-habits.md   Deciding, sharing evidence, the weekly habit
    ├── templates.md                 Copy-and-fill templates
    ├── pitfalls-and-limits.md       Anti-pattern checklist and where to adapt
    └── further-reading.md           Books for going deeper
```

`SKILL.md` stays short and loads first. Claude reads the reference files only when a step needs them.

## Principles in brief

1. Start with a goal and a question.
2. Customers don't design solutions.
3. Learn, don't validate.
4. Behavior beats opinion.
5. Keep it small, cheap, fast and ongoing.
6. Involve the whole team and share raw evidence.

## Scope and limits

- Discovery lowers the odds of building the wrong thing; it does not remove them. Treat every conclusion as the current best guess.
- It is built for teams and individuals of any size, with adjustments for brand-new products with no customers, regulated fields and heavy-process organizations (see `references/pitfalls-and-limits.md`).
- The skill does not cover roadmapping, delivery or other product management topics.
- It has been tried on a small number of realistic requests, not benchmarked.

## Further reading

The practices here follow widely used discovery literature. See `references/further-reading.md` for books that go deeper. The skill is an original synthesis in its own words and does not reproduce those works.

## License

Released under the [MIT License](LICENSE). You can use, copy, modify, share and sell it, as long as you keep the copyright notice.
