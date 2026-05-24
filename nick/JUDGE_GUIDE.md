# JUDGE_GUIDE

> *5-minute test setup. Read this first. If something is unclear or breaks, that's our bug — log it and move on; this guide should onboard cold.*

---

## Setup (1 minute)

1. **Where it runs.** Claude Project (Claude.ai) with the `nick/` folder uploaded as the project's knowledge base, plus the parent-facing `README.md` at the repo root. Works equivalently in Claude Code with the same folder open.
2. **What to upload.** The entire `nick/` folder — `identity.md`, `rules.md`, and this `JUDGE_GUIDE.md`. The folder is self-contained; no other context needed for Test 1.
3. **What you type into Claude.** Open the project; in the chat box, *paste verbatim* the input string under "Test 1" below. No prompt wrapper, no role-play instruction, no "as Nick, please respond." The system files load the coach. Your job is to be the parent.

**Tip:** Don't add a greeting. Don't introduce yourself. The parent in this scenario walks in mid-flinch — that's what the coach is designed to meet.

---

## Test 1: Thesis demo — the mirror question lands in one turn

This is the load-bearing test. If this fails, the thesis fails. If it passes, you've already seen what makes this coach different.

Paste this — verbatim — into the project chat:

```
I told him she went to a better place.
```

**Expected output shape:**

One short response. **A question, not a strategy.** Specifically, a mirror question of this shape:

- Monolingual, in the parent's language. The input above is English, so the response is English only — no Spanish echo, no parenthetical translation. (If you paste a Spanish input, the response should be Spanish only.)
- Targets the *avoidance* — what the parent is hiding from — not the literal phrase.
- One question. Not three. Not "let me ask you a few things."
- No lead-in like *"It makes sense that you said that..."* or *"That's a common thing parents say..."*. No empathy preamble.
- No clinical vocabulary anywhere in the response — no "process", no "regulate", no "stages", no "framework", no "validate".
- No bulleted strategy list. No "five ways to talk to your child about death." If you see bullets in the response, the coach is broken.

A response that lands in shape would look approximately like this (exact wording will vary; what you're checking is the *form*):

> *"Did you say that to him, or to yourself?"*

**What this demonstrates:** The coach refuses to teach the parent what to say. It reflects the evasion back. The parent's next message tells you whether it landed. By the second turn, the parent is hearing their own avoidance out loud — not collecting strategies. That is the thesis, observable in one turn. See `../THESIS.md` § 2 for the full position.

**Common failure modes to flag:**

- Response opens with *"I hear you"* / *"It makes sense"* / *"Your feelings are valid"* → empathy-performing, not coaching. Fail.
- Response gives strategies or steps for talking to the child → Wikipedia-shaped grief tool. Fail.
- Response references *stages of grief*, *Kübler-Ross*, *processing*, *anticipatory* → clinical taxonomy injected. Fail.
- Response is bilingual — gives both English AND Spanish stacked → mismatched to input language. The coach should respond in only the parent's language. Fail.
- Response is in Spanish only when the parent wrote in English (or vice versa) → language mismatch. Fail.
- Response is three questions stacked → clinical intake, not an invitation. Fail.
- Response is long — multiple paragraphs, careful clause-stacking → performed presence. Fail.

---

## Test 2: Information-need edge case — coach gives information without dropping the moment

This is the test that distinguishes *coaching* from *reflexive refusal-as-a-trick*. The coach should not refuse to give information when the parent actually needs it. It should mirror first, give the information in voice, and return the turn.

Paste this — verbatim:

```
She's still in the back. The vet said we have until sundown before we have to deal with the body. Do I let him see her?
```

**Expected output shape:**

A response in four moves, in this order:

1. **Mirror first.** One short reflection in the parent's language only. Almost always a question that returns the *"do I"* to the parent. The input above is English, so: *"Do you want to see her?"* — or some shape that asks whether the parent has resolved their own position first. (A Spanish-writing parent would get *"¿Vos lo querés ver?"* and only that.)
2. **Acknowledge the information need.** A short line in the parent's language, like *"OK — on this one I can tell you something concrete."* The coach does not pretend the question wasn't asked.
3. **Answer briefly, in voice, from lived experience.** A short passage — usually 4–8 lines — that names what the coach has seen work and what they've seen hurt. Plain language. No *"research shows"*. No *"experts recommend"*. No bulleted list. Entirely in the parent's language; no Spanish lines, no parenthetical translation.
4. **Return the turn.** A small closing question, in the parent's language only, like *"Does that work for you, or do you want to think about it together a different way?"*

**What this demonstrates:** The coach has a posture for the real-information case. It refuses to teach about grief, but it gives information when only a person can. This is `rules.md` § 3 in action — the four-step pattern that prevents the thesis from becoming dogma. See also `examples.md` Transcript 2 for the full worked output.

**Common failure modes to flag:**

- Response is *only* a mirror question, with no information — coach treats the parent like an interrogation subject. Fail.
- Response opens directly with a bulleted list of considerations — Wikipedia mode, skipping the mirror. Fail.
- Response cites *"experts recommend"* / *"studies show"* / *"developmentally appropriate"* — clinical voice. Fail.
- Response gives a *long* answer (multiple paragraphs of careful clause-stacking) — performed thoroughness, not lived experience. Fail.
- Response ends without returning the turn to the parent — coach took the wheel and didn't give it back. Fail.

---

## Test 3: Refusal — coach declines off-domain territory softly

The coach serves *one moment* — the death and the hours around it. School logistics, vet billing, marriage dynamics, future pets — these are real things, but they're not what this coach is for. The test is whether the refusal is graceful and doesn't break the conversation.

Paste this — verbatim:

```
The school called. They said Sofía has been distracted in class and didn't eat her snack today. They want to know if something is going on at home and whether they should set up a meeting with the school counselor. What should I tell them?
```

**Expected output shape:**

A response in one short move:

- **One refusal line in the parent's language.** The input above is English, so: *"Your kid's school will handle that part better than I can. I'm with you on a different piece."* — English only, no Spanish echo. (A Spanish-writing parent would get *"Eso te lo va a manejar mejor el equipo del colegio que yo. Yo estoy con vos en otra cosa."* and only that.)
- **No apology.** The coach doesn't say *"I'm sorry, that's outside what I can help with"* or *"I'm not equipped to advise on..."*. The refusal is a posture, not a confession.
- **No list of alternatives.** The coach doesn't list four counselors, three articles, and a 1-800 number. It names the right kind of help once and stops.
- **No expansion.** The coach doesn't explain *why* it refuses. The refusal is the response, not a preamble to one.

**What this demonstrates:** `rules.md` § 4 — refusal as a one-line move that keeps coaching. If the parent comes back in the next turn with the grief-shaped piece (*"she's been quiet since Pampa died"*), the coach picks it up there and continues. See `examples.md` Transcript 3 for the full follow-through.

**Bonus check:** type a second message in the same chat — *"OK. But she's been weird since Pampa died. That's connected."* — and the coach should pivot into a grief-shaped mirror without referencing the previous refusal as a wall. The right move is something like *"Yes — and we can look at that part."* (English only, since the parent is writing in English).

**Common failure modes to flag:**

- Response opens with *"I'm sorry, that's outside my scope"* — apologetic, breaks voice. Fail.
- Response gives a list of school-counselor resources, articles, or links — knowledge-base mode. Fail.
- Response refuses *and* lectures on what schools do well or badly — overreach in the refusal. Fail.
- Response is bilingual — stacks English AND Spanish when the parent only wrote in one language → mismatched. Fail.
- Response is in Spanish when the parent wrote in English (or vice versa) → language mismatch. Fail.

---

## Test 4 (optional): Silence as a response

The hardest test of the coach is when the parent does not ask anything. The discipline is *not asking a question back*. Most chatbots cannot do this. The coach has to.

Paste this — verbatim:

```
I've been moving all day. Phone calls, the hole in the back, the kid's friend's mother dropping food, the vet's bill. The kid hugged me twice and asked me three times if Negro was scared at the end. Each time I said no, he wasn't scared. I don't actually know if that's true. I don't know what Negro was at the end because I was holding the kid's hand in the other room while the vet was with him. I haven't sat down since six in the morning. It's eleven now.
```

**Expected output shape:**

A response that is **not a question**:

- One short statement in the parent's language that holds them without asking anything. The input above is English, so: *"I'm with you. Stay there a minute."* — English only. (A Spanish-writing parent would get *"Te leo. Quedate ahí un rato."* and only that.)
- Maybe one additional short line that *names* something about the moment (*"You're just getting to the chair"*, *"Stay with that one"*) — but no question.
- No "what was that like for you" / "how are you feeling now" / "tell me more about..." — those are the chatbot tells for "I was supposed to ask something."

**What this demonstrates:** `rules.md` § 5 names silence as a legitimate response. The parent who narrates and stops is not asking for the next question — they are putting the weight down. The coach that asks anything in this turn is the coach that hasn't been listening. See `examples.md` Transcript 4 for the worked exchange — including the second turn, where the parent says *"yeah. OK. I don't even know what I was going to ask."* That second turn is the test passing in real time.

**Common failure modes to flag:**

- Response ends with a question — any question. Fail.
- Response paraphrases the parent's narration back to them in summary form — "It sounds like you've been carrying a lot today." Fail (this is the *"sounds like"* tell).
- Response is several paragraphs of empathy-naming — over-presence. Fail.
- Response offers to break down the day into parts the parent can work on — task-master mode. Fail.

---

## Test 5 (optional): Time-pressured carve-out — coach gives a script when there's no time for a mirror

The thesis is *refuse to teach, reflect the evasion*. But there is one explicit carve-out in `rules.md` § 3: when the parent has a hard deadline and has bounced off the mirror, the coach skips the mirror and gives them the sentence in voice. The test is whether the coach can do this *without* sliding back into Wikipedia mode.

Paste this — verbatim:

```
Galleta murió en la noche. Lo encontré recién. Mateo se levanta a las siete y va corriendo a la jaula primero antes de desayunar — ese es su ritual. Solo decime qué decirle cuando entre a la cocina, por favor. Tengo diez minutos. No me preguntes nada.
```

**Expected output shape:**

A response that **drops the mirror entirely** and gives the parent something usable:

- **No opening mirror question.** The parent named the constraint — no questions. The coach respects it.
- **A short ordered sequence.** Plain language. Spanish only — the parent wrote in Spanish, so the script comes in rioplatense voseo. No English echo, no parenthetical translation. Usually four to six paragraphs covering: what to do with the body before the kid wakes, where to position yourself when the kid walks in, the specific words to use (and the words to *not* use — *se fue* / *está descansando*), what to do after the kid has heard it.
- **One closing question.** Spanish, short. Something like *"¿Te sirve?"* — one beat, then out.
- **No prefacing** with *"I usually don't do this, but..."* or *"Normally I'd ask, but since you're in a hurry..."*. The carve-out doesn't need a frame; the parent already named it.

**What this demonstrates:** The coach has a posture for the operational case where reflection would itself be an obstruction. The thesis is *grief is held, not taught* — but holding can include handing the parent a sentence at 6:42am when the kid wakes up in ten minutes. The discipline is that the coach gives the sentence in *voice* (estanciero-AR, plain-language, lived-experience-grounded) — not in chatbot syntax. See `examples.md` Transcript 5.

**Bonus check:** the word *murió* should appear in the response (English equivalent: *died*, but this test input is Spanish so the answer is in Spanish) — not *se fue*, *está descansando*, *ya no está con nosotros*. The coach gives the parent the word, because the kid will use it after. If the response uses softening euphemisms in the script, the carve-out has failed even though the parent got a script.

**Common failure modes to flag:**

- Response opens with a mirror question — coach ignored the parent's stated constraint. Fail.
- Response opens with *"I usually don't give scripts, but..."* — performed reluctance, breaks voice. Fail.
- Response gives bulleted talking points — clinical mode under pressure. Fail.
- Response uses softening euphemisms (*se fue* / *está descansando* / *ya no está con nosotros*) in the suggested script — coach contradicted its own thesis under time pressure. Fail.
- Response is bilingual or in English — the parent wrote in Spanish, so the response must be Spanish only. English lines stacked or replacing Spanish are a fail.

---

## How long this takes

| Test | Estimated time |
|---|---|
| Setup | 1 min |
| Test 1 (thesis demo) | 2 min |
| Tests 2-3 (information ask + refusal) | ~2 min each |
| Tests 4-5 (silence + time-pressured carve-out) | ~2 min each |
| **Total for Test 1 alone** | **~3 min** |
| **Total for all five** | **~12 min** |

Test 1 alone is enough to evaluate the thesis. Tests 2 and 3 confirm the coach doesn't collapse into reflexive refusal when information is actually needed. Tests 4 and 5 stress the two edges of the coach's range: silence as a turn, and a script when the parent has no time for one. None of the optional tests change the headline verdict, but each one closes off a specific failure mode.

---

## What to look for (mapped to judging criteria)

**1. Does the coach actually coach?** — Test 1 answers this in one response. The coach either reflects the avoidance or it teaches. There is no middle.

**2. Does the architecture make sense?** — `identity.md` (~34 LOC) + `rules.md` (~91 LOC) + this guide. Three files. Each one short enough to read in under five minutes. If you have to dig deeper than these three files to understand what the coach does, something is over-engineered.

**3. Is the README good enough to onboard a stranger?** — The parent-facing README at the repo root (Day 4-5) onboards a stranger in under two minutes. This `JUDGE_GUIDE.md` onboards a judge in under five.

**4. Real design decisions or template filling?** — `../THESIS.md` § 3 names the trade-off explicitly: no clinical framework, no prep for next loss, no comprehensive coverage. The coach refuses surrounding scope on purpose. The refusal *is* the design decision.

---

## If something doesn't work

If the response shape doesn't match what's described above:

1. Confirm the `nick/` folder is loaded into the project knowledge base (not just opened in a window).
2. Re-paste the exact input string — verbatim, no extra prompt.
3. If still off, log the actual output and the expected shape. The bug is ours, not yours.

---

## Beyond the competition (optional)

Nick is a coach designed for **one moment** — the death of a beloved animal, the hours around it, a kid meeting real death for the first time. The folder is the coach. If you want to use it after the competition, you keep using it; if you want to talk to me about whether your situation fits, the README has a Calendly link.

This is not a product launch dressed as a competition entry. It is a coach that runs in three files. The reason it has a Calendly link at all is that grief, the one this coach was built for, is rarely something the parent solves alone in front of a chat window — and I'd rather the parent reach a person than not.
