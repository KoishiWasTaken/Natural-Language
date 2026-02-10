# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Em dashes (—).** Most humans can't type them on a keyboard. Use commas, periods, hyphens (-), or start a new sentence instead.
- **Too-clean structure.** Two tidy paragraphs each making one distinct point reads like AI.
- **Uniform sentence length.** Mix short punchy fragments with longer ones.
- **Comprehensive coverage.** Don't cover every angle. Pick one and run with it.
- **Complete narrative arcs.** Telling stories in perfect chronological order with clean beginning-middle-end feels rehearsed. Real people skip details or jump around.
- **"There was actually..." transitions.** Known AI pivot phrase.
- **Overly smooth connective tissue.** "which makes it," "basically because," "so even"
- **Balanced, neutral presentation.** Real people have preferences and lead with them.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought, every time.
- **Consistent register throughout.** Real people shift register mid-thought.
- **Over-performing casualness.** Fake anecdotes, "lol," forced stream-of-consciousness = detectable "AI trying to sound human" pattern.
- **Fabricated personal memories.** Hedged fake memories feel constructed at the statistical level.
- **Excessive length.** 100-110 words is the sweet spot. Over ~120 tends to score worse.
- **One-point-per-paragraph lists.** Listicle in paragraph form.
- **Template/draft generation.** Embedded templates (emails, letters) are AI-detection poison.
- **Mixed-format responses.** Prose → template → more prose is textbook AI structure.
- **Clean topic splits.** Don't partition answers into neat categories.
- **Precise round numbers in casual context.** Use "like 80 hours" not "80 hours." The hedging word "like" before numbers is very human.

## Positive Elements

- **Casual opener.** Jump right into the answer informally. One-word sentence openers work great ("Hades.").
- **Conversational contractions.** "nobody's putting," "they'd both be right," "it's kind of watery," "you're not risking much"
- **Concrete references.** Specific names, numbers, details. Package them loosely.
- **Opinionated framing.** Lead with a strong personal take. Don't hedge or present both sides equally.
- **Varied sentence length.** Short fragments mixed with longer explanations.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts.
- **Throwaway closing lines.** Short, casual, don't summarize or wrap up neatly.
- **Brevity and punch.** 100-110 words. Say what you mean and stop.
- **Humor and irony.** Natural humor, not forced jokes.
- **Blunt, slightly rude tone.** "a stupid amount of content," "You'd sound ridiculous." AI is polite. Humans aren't always.
- **Regular punctuation only.** Commas, periods, hyphens, question marks. Nothing fancy.
- **Casual quantifiers.** "like 80 hours," "like 15 bucks" instead of precise numbers. This is how people actually talk.
- **No em dashes.** Confirmed in Round 10 alongside other improvements.

## Patterns and Observations

- **CONFIRMED: Topic type is the dominant variable.** Casual opinion questions pass all 5 detectors at 100+ words (Rounds 2-3 at 4/5 with em dashes, Round 10 at 5/5 without). Factual/narrative/educational topics fail ZeroGPT (60%+) and GPTZero (100%) regardless of style.
- **GPTZero IS beatable at 100+ words.** Round 10 proved it: 3% AI at ~110 words. The key was casual opinion topic + no em dashes + strong opinionated lead + informal quantifiers. Previous assumption that GPTZero was unbeatable at length was WRONG.
- **The winning formula (5/5 at 100+ words):**
  - Casual opinion topic (recommendations, preferences, subjective questions)
  - ~100-110 words
  - Strong opinionated lead (name something specific immediately)
  - No em dashes
  - Casual quantifiers ("like X")
  - Informal/slightly rude language ("a stupid amount," "you're not risking much")
  - Varied sentence length
  - No clean narrative arcs or topic partitions
  - Regular punctuation only
- **What still doesn't work at 100+ words:** Factual/educational/narrative topics. These may require a fundamentally different approach or may just be harder to disguise.
- Grammarly, Quillbot, and Copyleaks: trivially easy on conversational responses.
- ZeroGPT: 0% on opinion topics, 60%+ on factual topics. Topic type is the switch.
- GPTZero: Beatable on opinion topics with the right style. Unbeatable on factual topics at length.

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
| 10    | 0%        | 3%      | 0%       | 0%        | 0%      | 5/5       |

*Round 1 used Scribbr instead of Copyleaks
