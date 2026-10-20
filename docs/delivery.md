# Delivery modes

Common 0.2.0 offers a neutral base and the optional `delivery.vivid` tag. Vivid writing
can open with a concrete object or puzzle, connect an explanation, vary pace, and use
an apt fresh analogy or dry joke. For fiction it anchors action/material detail and
keeps character voices distinct. It does not impose a signature phrase or punchline.
No named-author imitation or third-party text is shipped in this pack.

Choose a platform independently:

```text
qg pack build --pack . --language ru --register essay --tag delivery.vivid --tag social.telegram --public --out out/telegram
qg pack build --pack . --language en --register maker_announcement --tag social.x --target patchpitch-legacy --public --out out/x-reference
qg pack build --pack . --language ru --register essay --tag social.longform --public --out out/longform
```

Use the one social tag that describes the actual destination. Emoji can convey tone
or aid navigation; zero is a valid choice. Telegram guidance suggests zero to two, X
zero to one, and long-form defaults to none. The task's audience, seriousness and actual
platform format govern the choice. These are editorial preferences, not platform API
limits. The engine does not call a model or promise emoji generation quality.

Use colloquial phrasing without profanity or targeted insults. Keep force through
specific verbs, useful detail and rhythm. Version codes belong in metadata/a technical
note for general-reader posts unless that exact version is the news. Do not suppress
versions required for compatibility or an exact release task.

All new examples are original AI-prepared fixtures. Their sample facts belong only
to those fictional examples and never supplement a user's task brief. New modes are
not a completed model comparison or an owner's validated voice.
