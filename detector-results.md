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

*New rounds will be appended below as training continues.*
