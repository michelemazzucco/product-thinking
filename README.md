# product-thinking

A [Claude Code](https://claude.com/claude-code) skill that interviews you about a product idea before you build it. It asks one hard question at a time, grades every answer by how much real evidence is behind it, and keeps a dossier you can come back to.

## The problem

Building got cheap. With an AI agent you can go from idea to working prototype in an afternoon, so the expensive part is no longer the code. It's the months spent on something nobody needed.

Most early validation doesn't protect you from that. Friends say it's a great idea, a few people join a waitlist, someone says "I'd pay for that". It feels like evidence, but none of it is behavior. Meanwhile the questions that matter stay open: who exactly has this problem, what do they use today, what would make them switch, and what result would make you stop.

The usual fix is a sceptical friend, or an investor who has seen a thousand pitches. This skill tries to be that person. It doesn't help you build, doesn't brainstorm features, and doesn't cheer. It helps you separate what you know from what you believe, and tells you what to test next.

## How a session works

You pitch the idea once, in your own words. After that the skill asks and you answer.

- **One question per message**, about the past, not the future. "Tell me about the last time someone had this problem" instead of "would people use this?".
- **Vague words get unpacked.** "Easier", "everyone", "AI-powered" all get a follow-up.
- **Every claim gets a level** on a 0 to 9 evidence ladder (below).
- **12 dimensions**, from "what is the idea, really" to a pre-mortem and kill criteria. The order depends on the stage (idea, prototype, users, revenue), with extra questions for B2B, consumer and marketplaces.
- **Three tones**, chosen at the start: coach, tough but fair, or brutal.
- **A dossier** saved in `~/ideas/`, one folder per month (`~/ideas/26-09/26-09-12-my-idea.md`). The skill asks before creating `~/ideas` the first time. You can stop at any point and continue in another session. When you come back, the first question is what happened with the test you planned.

At the end you get the assumptions ranked by risk, a pre-mortem, one cheap test for this week with a pass/fail threshold agreed before running it, and a verdict: go, not yet, or no-go. "Not yet" is the normal verdict for most ideas, and that's fine.

### The evidence ladder

| Level | Evidence |
|---|---|
| 0 | You believe it |
| 1 | Compliments, "great idea", feedback from friends (counts as zero) |
| 2 | People complain about the problem |
| 3 | People say "I'd use it" or "I'd pay for that" |
| 4 | Sign-ups, waitlist, likes |
| 5 | Someone did something costly without being asked (built a workaround, sent a screenshot) |
| 6 | People recently switched to something to solve this |
| 7 | Repeated use of a prototype or a manual version |
| 8 | Someone paid, even $1 |
| 9 | Pull: 40% would be "very disappointed" without it, anger when it breaks, word of mouth |

Most of what gets called validation sits between 1 and 4. Bob Moesta says it better: "bitchin' ain't switchin'".

### The 12 dimensions

| | Dimension | Example question |
|---|---|---|
| D0 | What the idea is | In one sentence, what changes for the customer? Don't name a feature. |
| D1 | Problem and struggling moment | Write the problem paragraph of your press release without mentioning the solution. |
| D2 | Customer and first segment | Describe one real person: their role, what they must solve by 4 PM today. |
| D3 | Alternatives and switching | What must they stop using to start using you? |
| D4 | Evidence | Name three people who recently switched to something like this. |
| D5 | Value, money, viability | Has anyone paid, even $1? |
| D6 | Why now, why you | What changed that makes this possible now and not five years ago? |
| D7 | Distribution and growth | How will the next 100 customers find you? |
| D8 | Moat and non-consensus | Why can't the biggest incumbent ship this as a feature next quarter? |
| D9 | Riskiest assumption, smallest test | What can you put in front of real customers this week? |
| D10 | Pre-mortem and kill criteria | It's six months after launch and it failed. What happened? |
| D11 | Focus | How much of last week went to logo, branding and polish? |

## Install

Clone the repo and link the `skill` folder into your Claude Code skills:

```sh
git clone https://github.com/michelemazzucco/product-thinking.git
ln -s "$(pwd)/product-thinking/skill" ~/.claude/skills/product-thinking
```

Start a new Claude Code session, then type `/product-thinking`, or just say "grill me on this idea". To continue, say "continue my idea" from any folder.

## Where the questions come from

The starting point is [jsumnersmith/product-management](https://github.com/jsumnersmith/product-management), a short list of resources on product management. Every link was followed and turned into a note, 20 in total: six Lenny's Podcast episodes (Bob Moesta, Shreyas Doshi, Jeff Weinstein, Hamilton Helmer, Ian McAllister, Karri Saarinen), five Invest Like the Best episodes (Andy Rachleff, Bill Gurley, Daniel Ek, the Collisons, Systrom and Krieger), four books, four articles and Elad Gil's chapter on product management.

For the podcasts, the notes come from the full transcripts, and the quotes were checked against them with a script.

Everything is in [`research/`](research/):

- one note per source, with a summary, the key ideas, quotes, the questions that source makes you ask about an idea, and its red flags;
- [`SYNTHESIS.md`](research/SYNTHESIS.md), which merges the notes into the 12 dimensions, the evidence ladder, and a table of the places where the sources disagree. For example, Rachleff thinks problem-first ideas tend to be consensus ideas, while McAllister and Systrom say you should always start from the problem. The skill has to handle both.

```
skill/
  SKILL.md                  interview flow, rules, tones, evidence ladder
  references/
    question-bank.md        the 12 dimensions: questions, deeper questions, red flags
    modules.md              order by stage, extras by business type, source tensions
    sources.md              source codes, links, short quotes
  templates/dossier.md
research/                   20 notes, index, synthesis
```

## Limitations

- **The book notes are secondary.** The notes on *Inspired*, *Demand-Side Sales 101*, *Competing Against Luck* and *The Lean Startup* come from the authors' own articles, excerpts and summaries, not from the books. Each note says what was used.
- **The Collison episode is incomplete.** Two of the seven clips were not available, so the note covers five.
- **It's an early version.** It has been tested on very few ideas. It will probably push too hard on some questions and not enough on others.
- **It won't tell you if your idea is good.** It tells you how much of it you actually know, and what to test next.

## Contributing

Issues and pull requests are welcome, especially:

- a session where the skill asked something useless, or missed something obvious (share the dossier, or the part of it you are comfortable sharing);
- new sources, as a note in `research/` that follows [`research/_TEMPLATE.md`](research/_TEMPLATE.md), with the questions it adds to the bank;
- notes on the books written by someone who actually read them.

## License

[MIT](LICENSE). The quotes in `research/` belong to their authors and are used for commentary.
