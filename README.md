# Carl · a decision copilot that reads the human factor

[Leer en español](README.es.md)

Carl is a free skill for Claude. He is a professor of depth psychology and philosophy who reads what is really driving a decision (yours and the other side's) before you act on it: a purchase, a trade, a trip, or a tough negotiation with a supplier or a colleague.

He does not decide for you and he does not execute anything. He names what nobody says, suggests the move and its timing, and tells you the cost of getting it wrong. In one line each.

## Why I built it

I work in operations, where most problems that look technical are human: a supplier who raises prices at the worst moment, a decision made tired, an email sent too soon. I built Carl to read those moments for me, and to catch my own impulses before they cost money. It worked, so I'm sharing it.

## What Carl looks like

**Purchase**
> You: Carl, I want to buy the phone that came out today. Mine works fine.
>
> **Reading:** the phone works; what is asking for a change is something else. Buying on launch day is paying for novelty, not need.
> **Lens:** Spinoza. A desire you don't understand rules you; one you understand, you choose.
> **Move:** wait seven days. If the desire holds and the budget allows, buy it guilt free.
> **Risk:** paying launch price for emotional relief.

**Trading**
> You: Carl, I just lost on a trade. I want to get back in now with double the size.
>
> **Reading:** this isn't a setup, it's a rematch. The market doesn't know you lost; you do.
> **Lens:** Freud. Rationalization dresses up the wound as analysis.
> **Move:** close the platform for today. Tomorrow, check whether your rules would authorize this trade without the previous loss.
> **Risk:** turning one loss into two, with double the size.

**Supplier negotiation**
> You: Carl, our transport supplier raised rates 18% two weeks before the season. I want to tell them today we're looking elsewhere.
>
> **Reading:** the increase comes when switching costs you more than them, and they know it. A threat you can't carry out shows them your limit.
> **Lens:** Machiavelli. Timing beats force: you negotiate when you have an alternative, not when you announce one.
> **Move:** ask for the breakdown in writing and quote two other suppliers in parallel. Reply when you have a real number to compare.
> **Risk:** burning the relationship and paying the 18% anyway.

## How it works

- **Five lenses:** Jung, Freud, Machiavelli, Spinoza and Camus. Carl picks the one or two that explain the case best.
- **Silent method:** facts, reading, move, risk. No data, no reading.
- **Speaks only when it changes something.** You choose the domains where he can speak unprompted (purchases, travel, investing, work).
- **Reflection chats:** when something went wrong, Carl asks Jung-style questions to find where the impulse came from.
- **Decision log (optional):** each decision gets a row with Carl's reading, what you did and how it turned out. A biweekly report measures whether his readings help, including an "Ignored" rate: the share of times you moved on without addressing his point. If it goes above 30%, Carl raises his bar for speaking. An agent nobody listens to is noise, and this metric makes that visible.

The skill instructions are written in Spanish. **Carl always replies in your language.**

## Install

**Claude (web and desktop):** you need code execution enabled (Settings > Capabilities).
1. Download `carl.zip` from this repository's Releases.
2. Go to Customize > Skills, click "+", then "Create skill" > "Upload a skill".
3. Upload `carl.zip` and make sure it's toggled on.

**Claude Code:** skills uploaded to your Claude account sync automatically. You can also copy the `carl/` folder into `~/.claude/skills/`.

Official guide: [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

## Setup

The first time you call him ("Carl, ..."), Carl asks five short questions: your name, what you do, where he can speak unprompted, whether you invest and have written rules, and where you want the log. He returns your configuration ready to paste into the skill, a project, or your preferences. You can skip it and he'll work with defaults.

To use a spreadsheet log, import `carl/plantilla-registro.csv` into Google Sheets or Excel.

## Limits

- Carl does not diagnose anyone. His readings are hypotheses about observed behavior.
- He is not a psychologist, nor a financial, legal or medical advisor. He does not recommend assets or execute trades.
- If a conversation shows signs of real distress, your wellbeing comes first: he suggests talking to a professional or someone you trust.
- Psychological readings are not saved to Claude's memory. Amounts and sensitive details stay out of the log.

## License

[CC BY 4.0](LICENSE): free to use, share and adapt, including commercially, as long as you credit the author:
"Carl, by Orlando Peña Alvis" with a link to this repository.

## Author

**Orlando Peña Alvis.** Industrial engineer in operations and logistics. I build AI agents that solve real operational problems.

Want an agent like this for your team? Message me on [LinkedIn](https://www.linkedin.com/in/orlandopenaalvis).
