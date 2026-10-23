# Quillgrain Voice Common

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

Version 0.4.2 seeks a conversational middle ground with optional situational irony, explicit boundaries on invented explanations and unsolicited calls to action. Version 0.4.1 refines the conversational default with quieter factual openings and a restrained announcement example. Version 0.4.0 makes the revised Russian voice active by default. It adds four original synthetic demonstrations, a fact/borrowed-phrase boundary, connected rhythm and scoped humor. English guidance is retained. This is a CANDIDATE editorial release; human preference and general writing quality are not validated.

See [delivery and upgrade notes](docs/delivery.md), including the changed RU example selection: omitting `examples.common` alone no longer disables the four default register examples. The pinned engine/lock is unchanged as a dependency; the new lock records the new pack digest. Existing consumers pinned to 0.3.0 keep their old identity and require an explicit upgrade/re-export.

Full source corpora and local inference evidence are kept outside this public checkout. No source joke, source plot or named-author imitation target is bundled. The pack is data only; it does not run retrieval, an LLM, or fine-tuning.

The owner accepted 0.4.2 as the current Russian editorial baseline after reviewing paired announcement outputs. This scoped decision is not general quality or factual validation: local trials still show invented explanations and confused event states. Review generated facts before publication; the pack remains CANDIDATE.

The optional research corpus is maintained separately in PRIVATE Quillgrain_Corpus,
with local checks and no CI. This public pack requires no access to it and keeps
its original synthetic examples. Renaming preserves `quillgrain.common`.
`releases/0.3.0` retains exact historical voice data for consumers pinned to it.
Current locks use Quillgrain 0.1.0rc4; the 0.4.2 editorial rules/examples are unchanged.
