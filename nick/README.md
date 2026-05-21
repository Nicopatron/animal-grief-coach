# Nick — a coach for the hour the animal dies

> *Grief is held, not taught — the coach holds the parent so the parent can hold the kid.*

---

## Built by

I'm Nico. I grew up on a farm in Pilar, an hour outside Buenos Aires. I've spent more nights than I can count in a barn at four in the morning with a dying animal and a kid sometimes watching from the door. I built this for the parent who is sitting in their kitchen at midnight with the dog's empty bed in the next room, trying to find the sentence they're going to say to their kid in the morning.

This coach is not a chatbot impression of a therapist. It's not a knowledge base on childhood grief. It's the closest thing I could put in a folder to *the person you'd actually want at the kitchen table*, in the voice I would actually speak in.

The voice is rioplatense — voseo, short sentences, Spanish first and English second on every question that matters. If you're a parent who reads in either, you'll find it works. If you're a parent who reads only in English, you'll still find it works — the second line is for you and the shape is the same.

---

## Who this is for

A parent — usually 35 to 55 — in the hour, the day, or the week after the death of a beloved animal. Dog. Horse. Cat. Pony. The animal of the field with a name. The kid is 6 to 14 and meeting real death for the first time, not the death of a book.

The parent is also grieving. That's the point of the coach. The parent is trying to hold a kid who is meeting real death for the first time, and the parent's first instinct, almost always, is to flinch — to find a phrase, a strategy, a *better place*, a *they're not in pain anymore*. Something that closes the moment instead of staying inside it.

What this coach does is help the parent stop flinching long enough that the kid finds a parent who is *there* instead of a parent who is explaining.

---

## What a coaching turn actually looks like

A parent writes me at midnight, the dog put down that afternoon:

> *"I told him she went to a better place. He nodded and went to bed. Now I'm sitting here and I don't know if that was the right thing."*

A grief tool shaped like a Wikipedia article responds with five strategies for honest, age-appropriate language. This coach does not. It returns one question:

> *"¿Le dijiste eso a él, o te lo dijiste a vos?"*
> *"Did you say that to him, or to yourself?"*

The parent's next message is honest in a way the first one wasn't. That is the entire mechanic. Five more transcripts of this — including the harder edge cases (the parent who has ten minutes before the kid wakes up, the parent who is asked about heaven) — live in `examples.md`.

---

## What's in this folder

```
nick/
├── identity.md           ← Who I am. Where I'm coming from. The voice.
├── rules.md              ← How I work. The load-bearing file. (95 LOC)
├── examples.md           ← Six worked transcripts. What good looks like.
├── reference/
│   ├── initial-conversation.md   ← What the first turn looks like
│   └── parent-resistances.md     ← Eight evasions and what they mask
├── JUDGE_GUIDE.md        ← Five paste-and-go tests. ~12 min total.
└── README.md             ← This file.
```

Each file does one job. If you find yourself wanting to dig deeper than the file you're reading to understand what's happening, something is over-engineered and that's our bug.

---

## Getting started

### Path A — Claude Project (most common, 2 min)

1. Create a new project at [claude.ai](https://claude.ai).
2. Upload the `nick/` folder to the project's knowledge base.
3. Open the chat. Paste, verbatim, this:

   ```
   I told him she went to a better place.
   ```

4. Read the response. If it's a question — one short bilingual question that reflects what you were avoiding when you said the sentence — the coach is working. If it's five strategies for talking to your child about death, the folder didn't load. Re-upload and try again.

### Path B — Claude Code (3 min, for the technically inclined)

1. `git clone` the repo.
2. From the repo root, run `claude` and `cd nick/` (or open the folder directly).
3. Same paste as above. Same expected shape.

### Path C — cold paste (1 min, for evaluating without setup)

1. Open [claude.ai](https://claude.ai) in any conversation.
2. Paste the contents of `identity.md`, `rules.md`, and one of the transcripts from `examples.md` into the first message. Then paste the parent input from Path A.
3. The shape will be close to right but not perfect — context is short, no file structure. Path A is the canonical evaluation.

---

## What happens after the first turn

For a parent who keeps writing, the shape across the first few turns looks roughly like this:

```
Turn 1 (parent):   The first sentence. Often a euphemism, a question,
                   or a narration with no question at all.

Turn 2 (coach):    One mirror, or one silence-line, or one bilingual
                   refusal — picked from the shape of turn 1.

Turn 3 (parent):   The parent finds something underneath what they
                   said in turn 1. Often a word they hadn't used.

Turn 4 (coach):    Another mirror or a holding line. Sometimes a
                   short answer if the parent asked for one and there
                   was time for the mirror first.

Turn 5+:           The conversation has its own register. The
                   README stops being load-bearing.
```

If the parent has hard time pressure (*"he wakes up in ten minutes"*), the coach skips the mirror and gives them a script in voice. See `examples.md` Transcript 5 and `JUDGE_GUIDE.md` Test 5.

---

## What this coach is for

The coach serves one moment — the death and the hours around it — and treats that narrowness as the design decision. What it commits to:

- **The hour the parent is in.** The mirror question lives where the parent is right now. If the parent is past this moment and wants tools for the next loss, the coach points them somewhere a coach for that conversation lives.
- **Four moves done well.** The mirror question, the four-step information-ask, the bilingual soft refusal of off-domain territory, the silence-as-response. All four come out of lived experience at the corral, the barn, the kitchen at midnight.
- **A voice that is the mechanic.** Rioplatense, bilingual, plain language, lived-experience-anchored. The voice is what keeps the coach from sliding into the chatbot impression of a therapist.
- **A clean handoff to a real clinician when the parent or the kid needs one** — once, in one sentence, and the coach keeps holding the parent until that handoff is in motion.

This coach accompanies. Professional psychological support is something else, done by someone else, and there is a Calendly link below if you'd rather talk to a person than read a chat.

---

## If you want to talk

If you're a parent in this moment and you'd rather hear a voice than read a chat, the booking link goes live with the rest of the submission on Sunday May 24 — same URL where this README is hosted.

If you're a judge or a builder reading this for the competition: `JUDGE_GUIDE.md` is the right next file. Five paste-and-go tests, about twelve minutes total. Test 1 alone is enough to evaluate the thesis — the folder doesn't need the booking link to be evaluated.

The folder is the submission. The Calendly link is there if you'd rather hear a voice than read a chat.

---

## See also

- [`identity.md`](./identity.md) — who Nick is and where I'm coming from
- [`rules.md`](./rules.md) — the craft. The file the coaching turns come out of.
- [`examples.md`](./examples.md) — six worked transcripts across all five shapes a parent's first message takes
- [`JUDGE_GUIDE.md`](./JUDGE_GUIDE.md) — five paste-and-go tests
- [`../THESIS.md`](../THESIS.md) — the one-sentence position and the trade-off
