# Example: first conversation with a personal trainer who works with older adults

This file shows both steps for one request: first the context questions, then the guide.

## Step 1: reply asking for context

Request: "Help me prepare an interview for a first meeting with a customer who is a personal trainer for elderly people."

> Got it: a first conversation with a personal trainer who works with older adults. Before I write the guide, a few things would make it fit your project:
>
> 1. **What are you exploring, and what decision will these conversations feed?** (For example an app for trainers, a service for older clients, or just an open problem area. Default: open exploration, no concrete idea yet.)
> 2. **Who is this trainer?** Independent or in a gym/clinic, and do you know them already? (Default: independent, a stranger doing you a favor.)
> 3. **What do you already know?** Earlier interviews, hypotheses, or an idea you want to test indirectly. (Default: nothing yet.)
> 4. **What do you most want to learn from this first meeting, and is anything off limits?** (Default: how they find, train and keep older clients, and where it is hard.)
>
> Unless you tell me otherwise I'll assume 45 minutes, a video call, and that you interview alone. Answer in a line each, or reply "defaults", and I'll write the full guide: learning goals, a timed run sheet with questions and follow-ups, and a pocket card.

## Step 2: the guide

Request context after answers: "defaults".

This is a model of the expected output: depth, format and tone. Rebuild the prompts for each new domain.

---

## Interview guide: first conversation with a trainer of older adults

**Purpose:** understand how independent trainers find, assess, train and keep older clients today, and where the work is hard, before deciding what to build.
**Participant:** personal trainer who currently works with adults roughly 65 and over.
**Duration and format:** 45 minutes, video call or in person. One person asks; one takes notes.
**Assumptions (correct me if wrong):** the trainer is independent or small-scale; you have no product to show yet; the trainer is a user of any tool you build and also a window into the older clients, who you will interview separately.

### Learning goals
1. How do trainers find, assess and plan for a new older client, and where does that process break down? *Decides which stage of the client journey to focus on.*
2. What do they use today to plan, track and communicate (paper, spreadsheets, messaging apps, other tools), and what does it cost them in time and money? *Decides whether a tool opportunity exists or the pain lies elsewhere.*
3. Who actually decides and pays (the older person, a family member, a clinic or residence), and why do clients stay or leave? *Decides who the customer is.*

### Beliefs to challenge (interviewer only)
- Trainers lack good ways to track progress with older clients.
- Families strongly influence whether an older person hires a trainer.
- Safety worries are the main barrier to starting.
- Surprising answer: tracking is not a pain at all, and the real difficulty is finding clients or keeping them motivated.

### Before the meeting
- Look up the trainer's public profile, specialty and where they work.
- Prepare consent for notes or recording; open the snapshot template.
- Decide the small ask for the end: an introduction to a client or a family member who would talk to you.

### Run sheet

| Min | Block | Main prompt | Probes | Listen for |
|---|---|---|---|---|
| 0-4 | Opening | "Thanks for your time. I'm learning how trainers work with older clients. I'm not selling anything, and there are no right answers. Is it OK if I take notes?" | | |
| 4-10 | Context | "How did you start working with older adults?" then "Walk me through last week." | How many clients? Where do you train them? Alone or with an organization? | Scale, setting, how work is organized |
| 10-24 | Story: new client | "Tell me about the last time you started with a brand-new older client." | Where did they come from? What happened in the first meeting? How did you find out what they could and couldn't do? Did anyone else take part (family, doctor)? What did you write down and where? How long did all that take? | Assessment steps, who is involved, time spent, anything improvised |
| 24-33 | Story: a client who left | "Think of an older client who stopped. Tell me what happened." | What happened in the weeks before? How did you notice? What did you do? Did anything bring clients back? | Retention causes, warning signs, actions taken |
| 33-39 | Tools and workarounds | "How did you plan and record your sessions with that client? Can you show me?" | What else have you tried? What did you stop using, and why? What does it cost you, in time or money? | Home-made solutions, switching costs, paid tools already in use |
| 39-43 | Money and decisions | "Who paid for the last client's sessions, and how did they decide to hire you?" | Who else was involved? What else did they consider? | Payer vs user, decision process, alternatives |
| 43-45 | Wrap-up | "Is there anything I should have asked?" "Could you introduce me to a client or family member who would be willing to talk?" | | Referral, follow-up, next step |

If time runs short, drop "Tools and workarounds" first, then shorten "Context".

### In-the-moment reminders
- Stay on one specific event; if they say "usually" or "always", ask for the last time.
- Do not describe or pitch an idea. If asked what you are building, say you are still learning about the work.
- "That would be great" or "I would use it": thank them, then ask how they handle it today.
- A feature request: ask when they last needed it and what they did instead.
- Do not ask for client names or health details; ask what the trainer did and adapted.
- Silence is fine; let them finish.

### After the meeting
- Write the snapshot the same day (opportunities in their own words, quotes, a mini timeline of the client journey).
- Mark which of the three learning goals were answered and which beliefs were challenged.
- Schedule the next interviews: two more trainers, plus older clients and a family member.

### Pocket card
1. "Tell me about the last time you started with a new older client."
2. "What happened in the first meeting? What did you write down, and where?"
3. "Tell me about a client who stopped. What happened before?"
4. "How do you plan and track sessions? Show me."
5. "Who paid, and how did they decide?"
6. "Anything I should have asked? Who else should I talk to?"

---

I made some assumptions (independent trainer, no prototype yet). If the trainer works inside a gym or clinic, or you already have a concept to test, tell me and I will adjust the guide.
