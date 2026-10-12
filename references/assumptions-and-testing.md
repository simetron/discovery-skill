# Assumptions and testing

## Contents
- Test assumptions, not ideas
- Surface assumptions
- Prioritize assumptions
- Design the test
- Test ladder
- Commitment signals
- Statistical and bias cautions
- Other techniques

## Test assumptions, not ideas

Every idea rests on assumptions about customers, behavior, technology and economics. An idea is too big to test directly. An assumption can be tested in days. Testing assumptions also lets you eliminate several ideas at once when they share one.

## Surface assumptions

For each shortlisted idea:
1. Story-map the experience: who does what, in what order, to get value.
2. At each step, list what must be true for it to work. Expect around 20 assumptions per idea.
3. Run a pre-mortem: imagine it is six months after launch and the effort failed. What went wrong?
4. Phrase each assumption as something that must be true, in positive wording (for example, "customers will remember their password", not "customers won't forget it").

Classify each assumption:

| Type | Question |
|---|---|
| Desirability (value) | Do customers want it and get value from it? |
| Usability | Can people find, understand and use it, including people with accessibility needs? |
| Feasibility | Can we build and operate it, including technical, legal, security and regulatory limits? |
| Viability | Does it work for the business: does revenue exceed cost, and do marketing, sales, support and finance work? |
| Ethical | Could it cause harm? What data does it collect and how is it used? |

A frequent mistake is focusing only on desirability and forgetting viability, or checking feasibility too early.

## Prioritize assumptions

Plot assumptions on a grid of **importance** (how much does the idea depend on it?) against **evidence** (how much do we already know?). Test the leap-of-faith assumptions first: important, with the least evidence. Pick the top two or three. For a brand-new product with no customers yet, desirability is usually the biggest unknown.

## Design the test

1. Test assumptions from several ideas together. This reduces confirmation bias and escalation of commitment.
2. Simulate the experience so people act instead of saying what they would do.
3. Set success criteria before running the test: how many people you will test and how many must show the behavior. Use counts of people, not percentages.
4. Agree how confident you need to be, scaled to the cost of being wrong.
5. Start small and iterate. Use the cheapest, lowest-fidelity test that answers the question.
6. Design tests you expect to pass, so a failure is a real red flag.
7. Interpret results against your criteria, never after the fact.
8. Remember that testing reduces risk but cannot prove an idea works. Small tests give false signals, so mix methods. Stop when the team is comfortable acting.

A test plan has: the assumption (as a statement), the method, the participants and how many, the success criteria, and the decision each outcome would trigger. A template is in `templates.md`.

## Test ladder

From cheapest and fastest to more costly. Start low and move up only as risk requires.

| Method | Best for |
|---|---|
| Existing analytics on current behavior | Checking whether the behavior already happens |
| One-question survey about behavior | Quick check of one specific assumption |
| Fake door, landing page or smoke test (advertise a feature or product that does not exist yet and measure interest) | Demand before anything is built |
| Unmoderated test of a low-fidelity prototype (participants complete tasks on their own time, recorded) | Desirability and usability |
| Moderated usability test: high-fidelity prototype, defined tasks, a note-taker, keep the user in "use" mode rather than "critique" mode, stay quiet and don't lead | Usability |
| Concierge test (deliver the service by hand) or Wizard of Oz (a working front end with people behind the scenes) | Value and usability before automating |
| Feasibility prototype (just enough code to settle a technical risk) | Technical risk |
| Live-data prototype, invite-only test or small A/B test (for example a small share of high-traffic users) | Quantitative value |
| Commitment test: letter of intent, pre-order, paid trial, introductions, reference | Whether interest is real |

Prototypes should cost far less than the finished product. Treat a "minimum viable product" as a learning prototype, not a shippable release. A clickable mock-up tests usability but does not prove value: people praise designs they will not use.

## Commitment signals

When testing a specific solution, real interest costs the customer something:
- **Time:** a scheduled follow-up, a trial, reviewing a prototype, bringing colleagues.
- **Reputation:** introductions to colleagues or decision-makers, a testimonial, being a named reference, joining a pilot.
- **Money:** a letter of intent, pre-order, deposit or paid trial.

Compliments and "let me know when it's ready" count for nothing. A declined request still teaches you something. Don't use commitment requests in the discovery interviews themselves; keep those for tests of a specific solution.

## Statistical and bias cautions

- Quantitative results need adequate sample size and statistical significance. Polished tools and attractive charts make weak results look conclusive.
- Qualitative work is done when the same patterns keep recurring.
- Surveys and A/B tests must not replace conversations with real people.
- Surveys are easy to run badly and always return answers, even to flawed questions, so bad results rarely reveal themselves. Keep them short, specific and about behavior, with success criteria set in advance.
- Everyone is biased, including you. Name your biases with the team, recruit a representative sample and review your own notes critically. Bias is a reason to be careful, not a reason to skip research.
- Skip focus groups: people know they are being watched, and group dynamics distort answers.
- Don't build a dedicated testing lab when remote tests would do.
- A rating scale is only a Likert scale if it has an agree-to-disagree range with a neutral midpoint and has been tested for significance. Otherwise treat it as an ordered scale, and use bar charts and the most common answer rather than averages.

## Other techniques

- **Product/market fit survey** (for products already in use): ask engaged users how they would feel if they could no longer use the product. As a rule of thumb, if more than about 40% say "very disappointed", fit is likely.
- **Qualitative value test:** a high-value activity where you combine an interview, a usability check and a test of willingness to pay with the same person.
