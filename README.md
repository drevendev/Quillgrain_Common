# Quillgrain Common

**Every voice has a grain.**

An independent, public, neutral voice data pack for
[Quillgrain](https://github.com/drevendev/Quillgrain). It supplies soft defaults and
original RU/EN examples. It does not prohibit dashes, metaphors, long sentences,
humour or first person. Adapt it to the task and reader.

All examples are explicitly **synthetic / AI-prepared original fixtures** under MIT.
They illustrate desired editorial choices; they are not measured human writing.
RU is the first acceptance language. EN examples are editorially prepared; comparative
model quality and owner preference have not been validated.

After installing the pinned engine described in CI:

```text
qg pack validate --pack .
qg pack build --pack . --register essay --language ru --public --out out/essay
qg pack build --pack . --register maker_announcement --language en --target patchpitch-legacy --out out/announcement
```

Registers: conversational, essay, fiction_narration, maker_announcement. Add
`--tag include_negative` only when you intentionally want the labelled negative
announcement example. `voice.json` is canonical; `examples/` and `VOICE.md` aid reading.
The lock detects stale engine/data versions. This pack contains no private corpus and
does not depend on an author's personal pack. Generated exports do not install consumers.

Version 0.2.0 adds optional [vivid delivery and social-platform guidance](docs/delivery.md).
Use `--tag delivery.vivid` and the appropriate `social.telegram`, `social.x`, or
`social.longform` tag. Emoji are contextual and optional. No named author is an
imitation target, and no source passages are included.
