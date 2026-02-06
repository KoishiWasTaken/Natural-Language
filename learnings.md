# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Too-clean structure.** Two tidy paragraphs that each make one point, with a smooth bridge between them, reads like AI. Real people meander more.
- **Uniform sentence length.** Mixing in some short punchy fragments alongside longer ones adds texture. Round 1 sentences were all medium-length — too consistent.
- **Comprehensive coverage.** Answering a simple question by covering every angle is over-thorough. A real person would pick one angle and run with it, or be less organized about covering multiple.
- **"There was actually..." transitions.** This phrasing is a known AI pattern. Sounds like a scripted pivot to a fun fact.
- **Overly smooth connective tissue.** Phrases like "which makes it," "basically because," "so even" — every sentence flowing logically into the next without any rough edges feels machine-generated.
- **Balanced, neutral presentation.** Listing options without favoring one makes it feel like a reference article. Real people have preferences and lead with them.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought is a pattern that persists across rounds. Even when content varies, the shape stays the same.
- **Consistent register throughout.** Staying at the same level of casualness the entire time might be a tell. Real people shift register mid-thought.
- **Over-performing casualness.** Leaning too hard into stream-of-consciousness, fake anecdotes, and internet-speak ("lol") creates a different but equally detectable pattern — the "AI trying to sound human" pattern. (Round 4 lesson.)
- **Fabricated personal memories.** Hedged fake memories ("I remember being maybe 8 or 9") and too-perfect narrative arcs feel constructed at the statistical level.
- **Excessive length.** Longer ≠ more human. Shorter, restrained responses (Rounds 2-3, 6) scored best. Don't ramble to seem human.
- **One-point-per-paragraph lists.** Essentially a listicle in paragraph form. Mixing multiple points within a paragraph feels less structured.
- **Template/draft generation.** Round 7 (email draft) scored 2/5 — worst by far. Embedded templates (emails, letters, cover letters, etc.) are an extremely common AI use case and detectors are heavily trained on them. The format itself is toxic to scores. Even wrapping it in casual advice doesn't help. Avoid any response that contains a formatted template or draft.
- **Mixed-format responses.** Advice → template → more advice is textbook AI structure. Switching between conversational prose and formatted content (like an email) within one response is a dead giveaway.

## Positive Elements

- **Casual opener.** Informal starts that jump right into an answer consistently pass detectors. ("Yeah, technically..." / "Oat milk, honestly." / "I mean, depends..." / "It's just a fancy word for...")
- **Conversational contractions and phrasing.** "nobody's putting," "they'd both be right," "it's kind of watery" — these read naturally.
- **Concrete references and analogies.** Specific details and comparisons add personality. Package them loosely, not neatly.
- **Opinionated framing.** Stating preferences and leading with a personal take reads much more human.
- **Varied sentence length.** Short fragments mixed with longer explanations consistently passes most detectors.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts — informality in the joints between ideas.
- **Throwaway closing lines.** Short, casual sign-offs that don't summarize or wrap up neatly.
- **Brevity and punch.** Round 6 (~75 words) scored the best overall — first 5/5. Short, direct, no filler. Say what you mean and stop.
- **Humor and irony.** The ironic observation in Round 6 ("colloquialism is the least colloquial word") was a strong human signal. Humor that emerges from the topic itself, not forced jokes.
- **Blunt, dismissive tone.** "You'd sound ridiculous." — short, opinionated, slightly rude. AI tends to be polite and thorough. Being a bit blunt helps.

## Patterns and Observations

- GPTZero cracked in Round 6 (2% AI) after being 100% for 5 straight rounds. The key difference: much shorter response, punchier style, ironic humor, and a blunt closing. However, response was under the 100+ word recommendation, so this needs validation at longer lengths.
- ZeroGPT crept to 21.66% in Round 6 — highest passing score. It seems to dislike very short responses. There may be a tension between what GPTZero and ZeroGPT want: GPTZero prefers shorter/punchier, ZeroGPT prefers moderate length.
- Grammarly and Copyleaks are easy to pass on conversational responses but BOTH failed on template generation (Round 7: Grammarly 46%, Copyleaks 100%).
- Quillbot is the only detector that has passed every single round including the template disaster. Least challenging detector.
- **Round 7 was a format problem, not a style problem.** The casual tone was fine — the email template embedded inside the response is what destroyed the scores. Template/draft content is AI-detection poison.
- **The GPTZero breakthrough factors (Round 6):**
  - Very short (~75 words vs 100-150 in other rounds)
  - High burstiness — sentence lengths varied wildly (3 words to 25 words)
  - Ironic/humorous observation
  - Blunt, slightly dismissive tone
  - No smooth transitions between ideas
  - Two paragraphs with very different vibes (explanatory → sarcastic)
- **Next round:** Go back to a conversational question-answer format. Avoid any prompt that requires generating a template or draft. Aim for ~100-120 words with Round 6 qualities to validate GPTZero at proper length.

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

*Round 1 used Scribbr instead of Copyleaks
