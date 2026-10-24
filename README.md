# Quillgrain Voice Common

**Every voice has a grain.**

An independent public voice data pack for [Quillgrain](https://github.com/drevendev/Quillgrain).
Version **0.5.0** revises the Russian editorial base and four original synthetic
before/after examples. The task determines tone, distance and genre; humor and
expressiveness remain available without becoming an obligatory formula.

Status: **CANDIDATE / human review pending**. Acceptance of 0.4.2 was scoped to that
iteration, not transferred to this release. English examples remain editorial
fixtures without a new empirical calibration. No model-weight training is involved.

```text
qg pack validate --pack .
qg pack build --pack . --register essay --language ru --public --out PRIVATE_OUTPUT/common-essay
qg pack build --pack . --register fiction_narration --language ru --examples none --public --out PRIVATE_OUTPUT/common-rules
qg pack build --pack . --register maker_announcement --language en --target patchpitch-legacy --public --out PRIVATE_OUTPUT/common-legacy
```

Registers: conversational, essay, fiction_narration and maker_announcement, RU/EN.
The new RU register examples are selected by default. Former positive RU examples remain
RETIRED. Add `include_negative` only to intentionally select the labelled negative
Russian announcement example. Source facts and fictional scenario facts are not
portable instructions, memories or claims about a new task.

All distributed demonstrations are **original synthetic / AI-prepared fixtures**
under MIT. The public pack includes no personal prose, private source metadata,
corpus dependency or real inference output. Private reference material informs
editorial decisions; it is not required to build this pack. Public CI uses only
public pack data and the pinned public engine **0.1.0rc4**.

`voice.json` is canonical. See [editorial intent](VOICE.md), [review decisions](docs/review-0.5.md)
and [delivery/upgrade notes](docs/delivery.md). Historical data in `releases/0.3.0`
and `releases/0.4.2` retain exact prior identities. A new version requires explicit
parent pins and re-export; it does not install or upgrade consumer applications.
