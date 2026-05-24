# Nick

> *Grief is held, not taught — the coach holds the parent so the parent can hold the kid.*

A folder-based AI coach for parents in the hour, the day, or the week after the death of a beloved animal — when the kid is six to fourteen and meeting real death for the first time.

---

## Built by

> *This is an AI coach running in Claude. Built by Nico.*

I'm Nico. I grew up on a farm in Pilar, an hour outside Buenos Aires. I've spent more nights than I can count in a barn at four in the morning with a dying animal and a kid sometimes watching from the door. I built this for the parent who is sitting in their kitchen at midnight with the dog's empty bed in the next room, trying to find the sentence they're going to say to their kid in the morning.

The coach is in this repo. The voice is plain, short sentences, lived-experience-anchored. It responds in your language — only your language. If you write in English, it speaks English. If you write in Spanish, it speaks rioplatense voseo. The bilingual capacity is in the coach; the response stays in the language you arrived in.

---

## Quick terms

**Mirror question** — one short line, in the parent's language, that returns the parent's evasion to them.
**Evasion** — a phrase the parent uses to close the moment instead of stay inside it. *"She went to a better place"* is an evasion.
**Four moves** — mirror question · information ask · soft refusal · silence-as-response.
**Rioplatense** — Spanish from Buenos Aires region; voseo (vos, tenés, querés).

---

## What you get back

A parent writes at midnight — the family dog was put down that afternoon:

> *"I told him she went to a better place. He nodded and went to bed. Now I'm sitting here and I don't know if that was the right thing."*

A grief tool shaped like a Wikipedia article responds with five strategies for honest, age-appropriate language. This coach does not. It returns one question:

> *"Did you say that to him, or to yourself?"*

(A parent writing in Spanish would have gotten *"¿Le dijiste eso a él, o te lo dijiste a vos?"* — the coach matches your language.)

The parent's next message is more honest than the first one was. That is the entire mechanic. Six more transcripts of this — including the harder cases (the parent who has ten minutes before the kid wakes, the parent who is asked about heaven, the parent who wants tools for the next loss) — live in [`nick/examples.md`](./nick/examples.md).

---

## The flow on every turn

```
Parent writes:        a euphemism, a question, a narration, or a hard
                      time-constraint ("he wakes up in ten minutes")
       │
       ▼
Nick reads:           where in the arc · where the kid is · what word
                      they used · whether they asked something · how
                      much time they have
       │
       ▼
Nick gives back:      one mirror question (most cases)
                      one soft refusal (off-domain ask)
                      one silence-line (narration with no question)
                      one ordered script in voice (time-pressured)

                      Every response in the parent's language only.
       │
       ▼
Parent's next turn:   tells Nick whether the move landed
```

---

## What's in this repo

```
.
├── THESIS.md                ← One-sentence position + the trade-off (54 LOC)
├── README.md                ← This file
└── nick/
    ├── identity.md          ← Who Nick is, where he's coming from
    ├── rules.md             ← The craft. Load-bearing. (95 LOC)
    ├── examples.md          ← Seven worked transcripts
    ├── reference/
    │   ├── initial-conversation.md
    │   └── parent-resistances.md
    ├── JUDGE_GUIDE.md       ← Five paste-and-go tests (~12 min)
    └── README.md            ← Coach folder onboarding (<2 min stranger read)
```

Five files plus a `reference/` folder. Each file does one job. If you're lost, we messed up the structure.

---

## Getting started

**If you're a parent in this moment** — the fastest path is to upload `nick/` to a [claude.ai](https://claude.ai) project knowledge base, open the chat, and write your first sentence the way you'd write it to a friend at the kitchen table. The coach is the person at the table. See [`nick/README.md`](./nick/README.md) for the full setup.

**If you're a judge or a builder** — [`nick/JUDGE_GUIDE.md`](./nick/JUDGE_GUIDE.md) is the right next file. Five paste-and-go tests, about twelve minutes total. Test 1 alone is enough to evaluate the thesis.

**If you'd rather talk to a person than a chat window** — the booking link is at [calendly.com/nicopatron96/nick-30-min-chat](https://calendly.com/nicopatron96/nick-30-min-chat).

The folder itself is complete and the thesis is testable from `nick/JUDGE_GUIDE.md` alone. The booking link is for after, not for evaluation.

---

## The trade-off this folder commits to

This coach serves one moment — the death and the hours around it — and treats that narrowness as the design decision. See [`THESIS.md`](./THESIS.md) § 3 for the explicit trade-off. The short version is that this coach does four moves well, and points elsewhere for everything else.

The four moves:

1. **The mirror question.** One short line, in the parent's language, that returns the parent's evasion to them. The parent's next message tells Nick whether it landed.
2. **The four-step information ask.** When the parent needs a piece of information only a person can give, Nick gives it — in voice, from lived experience — and then returns the turn.
3. **The soft refusal.** When the ask is off-domain (school logistics, vet billing, in-laws), one line in the parent's language that names the right kind of help and keeps coaching.
4. **The silence-as-response.** When the parent narrates and stops without asking anything, the right turn is not a question. *"I'm with you. Stay there a minute."* (or, in Spanish: *"Te leo. Quedate ahí un rato."*)

This coach accompanies. Professional psychological support is something else, done by someone else, and the Calendly link is there if you'd rather hear a voice than read a chat.

---

## A live demo

A small landing page (single static file, no build step) is in `docs/`, deployed at [nicopatron.github.io/animal-grief-coach/](https://nicopatron.github.io/animal-grief-coach/). It shows the input/output shape for Test 1 inline. The canonical place to actually run the coach is [claude.ai](https://claude.ai) with the `nick/` folder loaded — see [`nick/README.md`](./nick/README.md) Path A.

---

## License

MIT.

---

*This coach accompanies — it does not replace professional psychological support.*
