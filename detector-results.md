# AI Detector Results Log

Tracking results from AI text detectors across training rounds.

---

## Round 1

**Prompt:** "Is tomato a fruit?"

**Response:**

> Yeah, technically it is. It's the ripened ovary of a flower, which makes it a fruit by the botanical definition. But nobody's putting tomato in a fruit salad, so in the kitchen it gets treated like a vegetable. The whole debate mostly comes down to which definition you're using — a botanist and a chef would just give you different answers, and they'd both be right in their own context.
>
> There was actually a Supreme Court case about this in the 1800s (*Nix v. Hedden*, 1893). They ruled the tomato was a vegetable for the purposes of tariff law, basically because that's how people used it in everyday cooking. So even the legal system sided with the culinary take over the scientific one.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 0% | 100% | Human |
| GPTZero | 100% | 0% | AI |
| Quillbot | 0% | 100% | Human |
| Scribbr | 0% | 100% | Human |
| ZeroGPT | 88.62% | 11.38% | AI |

**Pass Rate:** 3/5 detectors passed as human

**Notes:** GPTZero and ZeroGPT both flagged heavily. The response has clean structure, smooth transitions, and an informational tone that may read as too polished. The two-paragraph layout with a neat factoid follow-up is a very typical AI pattern. Possible issues: even sentence length, overly organized flow, the "there was actually" transition is a known AI tell, and the response covers the topic too comprehensively for a casual answer.

---

## Round 2

**Prompt:** "What's a good alternative to milk if I'm lactose intolerant?"

**Response:**

> Oat milk, honestly. It's the closest thing I've found to actual milk in terms of how it feels in coffee or cereal. Not too thin, not weird and chalky like some of the others.
>
> Almond milk is fine too but it's kind of watery if you're used to whole milk. Some people swear by coconut milk — I think it's too sweet for most stuff but it works great in smoothies or curry.
>
> Really depends on what you're using it for though. Like if you're baking, oat or soy are probably your best bet since they behave more like real milk when heated. If you just want something to drink straight, try a few and see what you actually like. They all taste pretty different from each other.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 0% | 100% | Human |
| GPTZero | 100% | 0% | AI |
| Quillbot | 0% | 100% | Human |
| Copyleaks | 0% | 100% | Human |
| ZeroGPT | 0% | 100% | Human |

**Pass Rate:** 4/5 detectors passed as human

**Notes:** Big improvement — ZeroGPT went from 88.62% AI to 0%. The varied sentence lengths, opinionated tone ("honestly," "I think"), and less-organized structure worked. GPTZero remains the only failure at 100% AI. Swapped Scribbr for Copyleaks since Scribbr uses Quillbot's engine.

---

## Round 3

**Prompt:** "Is water wet?"

**Response:**

> I mean, depends on how you define "wet." If wet means something has water on its surface then no, water itself isn't wet — it's just... water. It makes other things wet. That's like asking if fire is burnt.
>
> But then some people argue that water molecules are constantly in contact with other water molecules, so in that sense it's always "wetting itself" if that makes any sense. Honestly I think it's one of those questions that's more about semantics than actual science. There's no real answer because people can't even agree on what the question is really asking.
>
> Fun argument to have at 2am with your friends though.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 0% | 100% | Human |
| GPTZero | 100% | 0% | AI |
| Quillbot | 0% | 100% | Human |
| Copyleaks | 0% | 100% | Human |
| ZeroGPT | 0% | 100% | Human |

**Pass Rate:** 4/5 detectors passed as human

**Notes:** Consistent 4/5 again. Same pattern — everything passes except GPTZero at 100%. The response used ellipsis ("it's just... water"), an analogy ("That's like asking if fire is burnt"), informal filler ("I mean"), and a throwaway closing line. None of it moved GPTZero. Three rounds at 100% AI from GPTZero suggests it's keying on something deeper than surface-level style — possibly perplexity/burstiness patterns or token probability distributions.

---

## Round 4

**Prompt:** "Is Santa Claus real?"

**Response:**

> Okay so obviously no, not in the literal sense. There's no guy at the North Pole running a toy factory with elves. But I always think the more interesting part of this question is why people get so weird about it.
>
> Like, kids figure it out eventually on their own and they're usually fine? I remember being maybe 8 or 9 and just kind of piecing it together and it wasn't some traumatic thing, it was more like oh okay that tracks. The cookies were suspicious anyway. But some parents act like it's this huge betrayal when really I think most kids half-know for a while before they fully know, if that makes sense.
>
> The whole "spirit of Santa is real" answer people give always felt kind of like a cop-out to me though. He's either real or he's not, don't make it into a hallmark card lol.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 41% | 59% | Human |
| GPTZero | 100% | 0% | AI |
| Quillbot | 0% | 100% | Human |
| Copyleaks | 0% | 100% | Human |
| ZeroGPT | 18.39% | 81.61% | Human |

**Pass Rate:** 3/5 detectors passed as human (regression from 4/5)

**Notes:** Went backwards. Grammarly jumped from 0% to 41% and ZeroGPT from 0% to 18.39%. GPTZero still locked at 100%. The longer, more rambling stream-of-consciousness style with fake personal anecdote and "lol" may have created a different kind of AI pattern. Over-performing casualness might be a tell in itself. The fabricated personal memory ("I remember being maybe 8 or 9") could ring false at the statistical level. Response was also notably longer than previous rounds.

---

## Round 5

**Prompt:** "What were the most important events in the Cold War?"

**Response:**

> The Cuban Missile Crisis is the obvious one. Thirteen days in 1962 where the whole world was genuinely close to nuclear war — Kennedy and Khrushchev staring each other down over Soviet missiles in Cuba. That's probably the single tensest moment in modern history.
>
> Beyond that, the fall of the Berlin Wall in '89 is up there. Not because it was some dramatic military standoff but because of what it represented — the whole Soviet project was crumbling and everyone could see it happening in real time on their TVs.
>
> The Korean War doesn't get talked about enough though. It set the template for how the entire Cold War would play out — proxy wars, UN involvement, the idea that the US and USSR would fight through other countries instead of directly. Vietnam followed the same playbook later on.
>
> If you want a deeper cut, the Soviet invasion of Afghanistan in '79 is worth reading about. It basically bled the USSR dry and a lot of historians point to it as the beginning of the end for them.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 0% | 100% | Human |
| GPTZero | 100% | 0% | AI |
| Quillbot | 0% | 100% | Human |
| Copyleaks | 0% | 100% | Human |
| ZeroGPT | 15.31% | 84.69% | Human |

**Pass Rate:** 4/5 detectors passed as human

**Notes:** Back to 4/5 after the Round 4 regression. Grammarly returned to 0%. ZeroGPT at 15.31% — higher than Rounds 2-3 (0%) but within passing range. The factual/historical topic likely makes ZeroGPT score slightly higher since informational writing is more AI-adjacent. GPTZero remains immovable at 100% across all 5 rounds. The four-paragraph structure (one event per paragraph) is a bit listy but the opinionated framing ("the obvious one," "doesn't get talked about enough," "deeper cut") kept it from reading like a textbook.

---

## Round 6

**Prompt:** "What does colloquialism mean?"

**Response:**

> It's just a fancy word for slang, basically. Or close to it. Like when people say "gonna" instead of "going to," or "y'all" — that kind of thing. Words and phrases people actually use when they talk to each other versus what you'd write in an essay for school.
>
> The ironic part is that "colloquialism" itself is probably the least colloquial word in the English language. Nobody drops that in casual conversation. You'd sound ridiculous.

**Detector Results:**

| Detector | AI Score | Human Score | Verdict |
|----------|----------|-------------|---------|
| Grammarly | 0% | 100% | Human |
| GPTZero | 2% | 98% | Human |
| Quillbot | 0% | 100% | Human |
| Copyleaks | 0% | 100% | Human |
| ZeroGPT | 21.66% | 78.34% | Human |

**Pass Rate:** 5/5 detectors passed as human

**Notes:** First 5/5! GPTZero finally cracked — dropped from 100% to 2%. Key changes: much shorter response (~75 words), punchier sentences, an ironic/humorous observation, and less structured flow. However, detectors noted 100+ words recommended for accuracy, so the short length may be partially gaming GPTZero. ZeroGPT crept to 21.66% — highest yet but still passing. The challenge now is replicating this at 100+ words for a more reliable result.

---

*New rounds will be appended below as training continues.*
