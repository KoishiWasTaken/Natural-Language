# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Em dashes (—).** Most humans don't know how to type them. Use commas, periods, hyphens (-), or start a new sentence. Still worth avoiding even though Round 9 showed they aren't the sole ZeroGPT problem.
- **Too-clean structure.** Two tidy paragraphs that each make one point reads like AI.
- **Uniform sentence length.** Mix short punchy fragments with longer ones.
- **Comprehensive coverage.** Don't cover every angle. Pick one and run with it.
- **Complete narrative arcs.** Round 9 told the Nutty Putty story in perfect chronological order with a clean beginning-middle-end. Real people skip details, get parts wrong, or jump around in the timeline. Don't tell stories in a way that feels rehearsed.
- **"There was actually..." transitions.** Known AI pivot phrase.
- **Overly smooth connective tissue.** "which makes it," "basically because," "so even"
- **Balanced, neutral presentation.** Real people have preferences and lead with them.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought, every time.
- **Consistent register throughout.** Real people shift register mid-thought.
- **Over-performing casualness.** Fake anecdotes, "lol," forced stream-of-consciousness = "AI trying to sound human" pattern. (Round 4.)
- **Fabricated personal memories.** Hedged fake memories feel constructed.
- **Excessive length.** Best scores came from shorter responses. ~75 words (Round 6) was the only 5/5. Anything over ~120 words tends to score worse.
- **One-point-per-paragraph lists.** Listicle in paragraph form.
- **Template/draft generation.** Embedded templates are AI-detection poison. (Round 7: 2/5.)
- **Mixed-format responses.** Advice → template → more advice is textbook AI.
- **Clean topic splits.** Don't partition answers into neat categories.
- **Educational/factual/narrative topics at length.** Informational writing at 100+ words consistently scores high on ZeroGPT (60-66%). The only way to score well on these topics seems to be keeping them very short (Round 6).

## Positive Elements

- **Casual opener.** Jump right into the answer informally.
- **Conversational contractions.** "nobody's putting," "they'd both be right," "it's kind of watery"
- **Concrete references and analogies.** Package them loosely, not neatly.
- **Opinionated framing.** Lead with a personal take.
- **Varied sentence length.** Short fragments mixed with longer explanations.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts.
- **Throwaway closing lines.** Short, casual, don't summarize.
- **Brevity and punch.** Say what you mean and stop. Less is more.
- **Humor and irony.** Humor that emerges naturally from the topic.
- **Blunt, dismissive tone.** Being a bit rude or dismissive reads as human.
- **Regular punctuation only.** Commas, periods, hyphens, question marks. Nothing fancy.

## Patterns and Observations

- **GPTZero is essentially unbeatable at 100+ words.** Round 6 (2% at ~75 words) is the only success. Every round at 100+ words = 100% AI. This may be a fundamental limitation.
- **ZeroGPT has two modes:** 0% on casual opinion questions at moderate length (Rounds 2-3), and 60%+ on factual/narrative topics at any length (Rounds 8-9). Topic type matters more than style for ZeroGPT.
- **Em dashes are worth avoiding but aren't the main problem.** Removing them in Round 9 only moved ZeroGPT from 65.55% to 60.19%.
- **The Round 6 formula remains the only 5/5:** ~75 words, high burstiness, ironic humor, blunt/dismissive, no narrative arc, two paragraphs with different vibes. But it fails the 100+ word accuracy threshold.
- **Factual storytelling is inherently hard.** Telling a story in order, with correct details, at 100+ words will almost always flag ZeroGPT and GPTZero. This may be unsolvable within those constraints.
- Grammarly, Quillbot, and Copyleaks: trivially easy on conversational responses.
- **Next round:** Try a casual opinion question again (like Rounds 2-3) to confirm that topic type is the variable. No em dashes. ~100 words. See if ZeroGPT returns to 0% and if GPTZero improves at all.

## Score Tracker

| Round | Grammarly | GPTZero | Quillbot | Copyleaks | ZeroGPT | Pass Rate |
|-------|-----------|---------|----------|-----------|---------|-----------|
| 1     | 0%        | 100%    | 0%       | 0%*       | 88.62%  | 3/5       |
| 2     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 3     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 4     | 41%       | 100%    | 0%       | 0%        | 18.39%  | 3/5       |
| 5     | 0%        | 100%    | 0%       | 0%        | 15.31%  | 4/5       |
| 6     | 0%        | 2%      | 0%       | 0%        | 21.66%  | 5/5       |
| 7     | 46%       | 100%    | 0%       | 100%      | 72.83%  | 2/5       |
| 8     | 0%        | 100%    | 0%       | 0%        | 65.55%  | 3/5       |
| 9     | 0%        | 100%    | 0%       | 0%        | 60.19%  | 3/5       |

*Round 1 used Scribbr instead of Copyleaks
