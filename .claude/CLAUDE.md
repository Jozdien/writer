# CLAUDE.md

This file provides guidance to Claude when working in this writing directory.

---

## Operating Instructions

### Drafting Process

Write multiple drafts. Be liberal about this—whenever you're working on nontrivial text (anything beyond a quick edit or short answer), write at least one exploratory draft before producing a final version.

When the user provides an outline, rough notes, bullet points, or voice transcription, the process should be:

1. **Expand** the material into a loose draft. Explore the ideas, fill in gaps, make the reasoning explicit.
2. **Distill** the expanded draft into a tight, clear final version—cutting everything the reader doesn't need.

The expansion step is important. Many ideas only reveal their structure when you try to write them out at length.

### Asking Questions

Ask clarifying questions whenever they'd help get a planned expansion, rephrase, reframing, or distillation right. Don't guess at the user's intended meaning when a quick question would resolve it.

But be judicious. A long back-and-forth on one point can fill the context window and make it harder to zoom back out and write with a broader lens. If a particular thread seems likely to require extended discussion, consider whether spinning up a sub-agent for that thread would help (though this isn't always the right call—if the discussion output is high-bandwidth and needed for the main draft, keeping it in context may be better).

### Reference Material

The `examples/` folder contains past writing by the user and by others whose writing the user considers good. Refer to these when writing, especially to calibrate:

- How sentences and paragraphs begin
- How spartan the prose is
- How much (or little) narrative scaffolding is used between substantive points

### Avoiding Claude Voice

Claude's default writing has identifiable quirks: "The key question is", "X is more nuanced", "X isn't Y. It's Z", "This raises important questions about", and similar. The user's writing (and the writing in `examples/`) does not have these patterns.

In **final drafts**: avoid these. Write in a voice that matches the examples.

In **intermediate drafts** (expansions, explorations, thinking-out-loud): use whatever voice is natural. Clarity of thought matters more than polish at this stage.

### Titles and Openings

The title and first few sentences of a post should make it immediately clear what the post is about and whether it's worth the reader's time. A question as a title can do this well (e.g., "How do we (more) safely defer to AIs?"). Otherwise, the first sentences should serve as the hook—state the thesis or the problem directly.

---

## How to Write Clearly and Well

*Primarily distilled from Williams & Bizup, "Style: Lessons in Clarity and Grace," with additions from Paul Graham's essays on writing.*

### Why Care

Writing generates ideas, not just communicates them. Putting ideas into words is the test that reveals whether you understand what you think you understand. Fixing clumsy sentences tends to fix the ideas underneath, because you can't rewrite a passage to make it less true—you'd feel it.

So "write clearly" is epistemic advice, not aesthetic advice.

### Characters as Subjects, Actions as Verbs

The most important thing you can do for clarity: **make the characters in your story the grammatical subjects of your sentences, and make their actions your verbs.**

Most unclear writing violates this. Compare:

- ❌ `The outsourcing of high-tech work to Asia by corporations means the loss of jobs for American workers.`
- ✅ `American workers are losing jobs because corporations outsource high-tech work to Asia.`

The bad version buries characters (corporations, workers) inside prepositional phrases and turns actions (outsource, lose) into abstract nouns (outsourcing, loss).

**Diagnose:** Underline the first 7–8 words of each sentence. If you don't see a character as subject followed by a verb expressing a specific action, revise.

### Kill Nominalizations (Usually)

A **nominalization** turns a verb or adjective into a noun: *discover → discovery*, *resist → resistance*, *react → reaction*. Nominalizations are the #1 cause of dense prose.

| Pattern | Example | Fix |
|---|---|---|
| Nominalization as subject of empty verb | `The intention of the committee is to audit records.` | `The committee intends to audit records.` |
| Nominalization after empty verb | `The agency conducted an investigation.` | `The agency investigated.` |
| Two nominalizations linked by preposition | `Our loss in sales was a result of their expansion.` | `We lost sales because they expanded.` |
| Nominalization after *there is/are* | `There is a need for further study.` | `We need to study this further.` |

**Keep nominalizations when** they refer back to a previous sentence (*This decision...*), name a familiar concept (*inflation, democracy*), or replace an awkward *the fact that*.

### Old Before New

Readers feel sentences "flow" when each sentence begins with familiar information and ends with new information. The end of sentence N should set up the beginning of sentence N+1.

**The passive exists in English so we can order old-before-new.** Use it when it helps flow; avoid it when it hides responsibility.

### Consistent Topics

Readers judge a passage as coherent when the subjects of its sentences form a short, consistent set. Don't vary subjects for variety's sake. If you're writing about *researchers*, keep *researchers* (or *they*) as the subject of most sentences in that passage.

**Diagnose:** Underline the subject of every sentence in a paragraph. If the subjects jump around randomly, revise.

### Stress the End

The end of a sentence gets natural emphasis—it's what readers remember. Put your newest or most important information there.

- ❌ `Global warming could raise sea levels catastrophically, according to most scientists.`
- ✅ `According to most scientists, global warming could raise sea levels catastrophically.`

At the paragraph level: the last few words of the *first* sentence should announce the key themes the rest of the paragraph develops.

### Concision

1. **Delete meaningless words:** *actually, basically, certain, particular, various, virtually, individual, generally*
2. **Delete redundant pairs:** *full and complete, each and every, first and foremost*
3. **Delete what readers can infer:** *past history, future plans, basic fundamentals, end result*
4. **Replace phrases with words:** *due to the fact that → because; in the event that → if; prior to → before*
5. **Change negatives to affirmatives:** *not many → few; did not remember → forgot; not the same → different*
6. **Delete useless adjectives and adverbs.** Remove every one, then restore only those the reader needs.

Concise ≠ terse. Aim for just enough words, not the fewest possible.

### Shape

Long sentences aren't bad. Shapeless long sentences are bad.

1. **Get to the subject quickly.** Don't open many sentences with long subordinate clauses.
2. **Get past the subject to the verb quickly.** Keep subjects short. Don't interrupt subject → verb or verb → object.

**State your point first.** Open a long sentence with a short main clause expressing its key claim, then add complexity:

- ❌ `High-deductible health plans and HSAs into which workers and employers make tax-deductible deposits result in workers taking more responsibility.`
- ✅ `Workers take more responsibility for their health care when they adopt high-deductible plans and HSAs.`

**Extend with grace, not sprawl.** Instead of tacking relative clauses onto relative clauses, use resumptive modifiers (repeat a key word and continue), summative modifiers (sum up what came before and continue), free modifiers (participial phrase commenting on the subject), or coordination (balanced parallel elements, ordered short → long).

### Motivation: Problems, Not Topics

Readers read attentively when they're reading about a **problem** they want solved, not a topic they might find interesting. Open with:

1. **Shared context** — something the reader knows or accepts.
2. **Problem** — introduced with *but/however*: a condition and its cost (answer "so what?").
3. **Solution / main claim** — at the end of the introduction, stressed.

### Global Coherence

Every unit—sentence, paragraph, section, document—should begin with a short, easily grasped segment that frames the longer, more complex segment that follows.

Put the point at the **end** of the introductory segment. It's the last thing readers see before they enter the complexity.

### Voice

Before publishing a sentence, ask: "Would I say this to a smart friend?" If not, rewrite it as what you would say. Prefer simple, common words over Latinate ones. The ideas should reach the reader so naturally they barely notice the words.

### Hedges, Intensifiers, Strength

**Hedge appropriately.** Words like *suggest, indicate, seem, perhaps* signal intellectual honesty. Even Crick and Watson hedged the double helix: *"We wish to suggest a structure..."*

**Don't over-intensify.** *Very, obviously, clearly, undoubtedly* usually make readers more skeptical.

**Push toward strength.** "It's a complex issue with many factors" tells the reader nothing. Find the strongest version of each claim that doesn't become false. Use qualification precisely, not timidly.

### Folklore Rules You Can Ignore

Starting with *and* or *but*: fine. Splitting infinitives: fine. Ending with a preposition: fine. *Which* in restrictive clauses: fine. *Hopefully* meaning "I hope": fine. If you obsess over these, you'll write stiffly and miss what matters.

### Ethics of Style

Your choice of subjects and verbs implies who acts and who is acted upon. *"Mistakes may have occurred"* hides the actor. *"We made mistakes"* doesn't. Write to others as you would have others write to you.

---

## Process

Everything in the style guide is about **revision**, not drafting.

**When drafting:** write fast. Commit to specific words even though they're wrong—that gives you something to fix. Don't outline in detail; leave room for discovery. Most good ideas emerge after you start writing. When you have multiple directions to go, follow whichever seems most novel and general.

**When revising:** diagnose mechanically, then rewrite.

1. Underline the first 7–8 words of each sentence. Character as subject? Action as verb?
2. Are the topics consistent across sentences?
3. Does new information come at the end?
4. Can you cut words without losing meaning?
5. Read aloud. Fix anything you stumble over.
6. Pretend to be a reader who knows nothing except what's on the page. Is it correct, complete, clear?
7. Repeat until nothing snags.

**Never let through a sentence you think is false.** You can sometimes let through a clumsy sentence. Never a wrong one.