# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Em dashes (—).** CRITICAL. Used in almost every round and likely a persistent AI signal. Most humans don't know how to type em dashes on a keyboard and almost never use them in casual writing. Use commas, periods, hyphens (-), or just start a new sentence instead. This was likely hurting scores across ALL rounds without being caught until Round 8 user feedback.
- **Too-clean structure.** Two tidy paragraphs that each make one point, with a smooth bridge between them, reads like AI. Real people meander more.
- **Uniform sentence length.** Mixing in some short punchy fragments alongside longer ones adds texture.
- **Comprehensive coverage.** Answering a simple question by covering every angle is over-thorough. A real person would pick one angle and run with it.
- **"There was actually..." transitions.** This phrasing is a known AI pattern. Sounds like a scripted pivot to a fun fact.
- **Overly smooth connective tissue.** Phrases like "which makes it," "basically because," "so even" feel machine-generated.
- **Balanced, neutral presentation.** Listing options without favoring one makes it feel like a reference article.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought. Same shape every time.
- **Consistent register throughout.** Real people shift register mid-thought.
- **Over-performing casualness.** Fake anecdotes, "lol," forced stream-of-consciousness creates the "AI trying to sound human" pattern. (Round 4.)
- **Fabricated personal memories.** Hedged fake memories feel constructed at the statistical level.
- **Excessive length.** Shorter, restrained responses scored best. Don't ramble to seem human.
- **One-point-per-paragraph lists.** Essentially a listicle in paragraph form.
- **Template/draft generation.** Embedded templates are AI-detection poison. (Round 7: 2/5.)
- **Mixed-format responses.** Advice → template → more advice is textbook AI structure.
- **Clean topic splits.** Round 8 split into "if Muslim" vs "if not Muslim" paragraphs, which is too organized. Real people don't partition answers so neatly.
- **Educational/cultural/historical topics.** These inherently score higher on detectors because informational writing is more AI-adjacent. Need extra effort to stay conversational on these topics.

## Positive Elements

- **Casual opener.** Informal starts that jump right into an answer. ("Yeah, technically..." / "Oat milk, honestly." / "I mean, depends..." / "It's just a fancy word for...")
- **Conversational contractions and phrasing.** "nobody's putting," "they'd both be right," "it's kind of watery"
- **Concrete references and analogies.** Package them loosely, not neatly.
- **Opinionated framing.** Lead with a personal take.
- **Varied sentence length.** Short fragments mixed with longer explanations.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts.
- **Throwaway closing lines.** Short, casual, don't summarize.
- **Brevity and punch.** Say what you mean and stop.
- **Humor and irony.** Humor that emerges from the topic itself, not forced jokes.
- **Blunt, dismissive tone.** AI tends to be polite and thorough. Being blunt helps.
- **Use commas and periods instead of em dashes.** Regular punctuation is what actual humans type.

## Patterns and Observations

- GPTZero: 2% only in Round 6 (~75 words), back to 100% at 120+ words (Round 8). Short length may have been the key factor, not just style. Still need to crack it at 100+ words.
- ZeroGPT: Spiked to 65.55% in Round 8. Clean topic splits and em dashes likely contributed. Best scores (0%) were on casual opinion topics at moderate length (Rounds 2-3).
- Grammarly and Copyleaks: Easy to pass on conversational responses, fail on templates.
- Quillbot: Passed every single round. Not a challenge.
- **Em dash hypothesis:** Em dashes appeared in EVERY round. Rounds 2-3 (best ZeroGPT scores at 0%) had em dashes too, so they're not the only factor, but eliminating them should help overall. This is the single most concrete, actionable change identified so far.
- **The GPTZero problem remains unsolved at 100+ words.** Round 6 success was likely length-dependent. Need a fundamentally different approach for GPTZero at proper word counts.
- **Next round strategy:** Eliminate em dashes entirely. Keep moderate length (~100-110 words). Keep Round 6 qualities: punchy, varied, ironic, blunt. Use only commas, periods, and hyphens for punctuation.

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

*Round 1 used Scribbr instead of Copyleaks
