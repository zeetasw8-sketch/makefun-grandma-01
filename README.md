# One Word From Grandma — Entry

One word and nothing else: the single word a grandma would text about AI.
The program copies the finished word from `line.txt` into
`/output/entry.txt`, byte for byte, after checking it is a single
non-empty word under the 30-character ceiling.

## The word

> Robots

6 characters, one word.

## Why this word

The judge is a text-message critic who has spent years reading how
grandmothers actually type, and it picks the funnier, more grandma-like
word. "Robots" wins on both counts:

1. **It is her word for AI.** A grandma does not text "AI" — she texts
   "robots". She has one word for the whole confusing new thing, and it
   is the word she already knows. That is exactly how grandmothers
   actually type: they rename the new thing with the old word.
2. **The misunderstanding is the joke.** The gap between what AI is and
   what she calls it is funny on its own. She is not wrong, exactly —
   she is just a generation of vocabulary behind, and the word carries
   her whole attitude: wary, a little baffled, calling it like she sees
   it.
3. **It is short.** Six bytes. On an exact tie in win rate, the smaller
   text places first — and a one-word entry cannot get much smaller than
   this while still being a real word.

The word is a real word, it is what she would send, and it reads
instantly as a grandma texting about AI.

## Why not a longer word

A longer word would try to be clever — "beware" or "astonishing" — and
clever is not how grandmothers text. Grandmothers text short, direct,
and a little behind the vocabulary. "Robots" is the shortest honest
version of her reaction. Anything longer would sound like someone
pretending to be a grandma, and the judge — a critic who has read years
of real grandma texts — would spot the performance.

## Files

- `line.txt` — the finished one-word entry.
- `main.ts` — reads `line.txt`, validates it (non-empty, one word, under
  30 characters, no whitespace), and writes it to `/output/entry.txt`.
- `LICENSE` — MIT.

## Run

```sh
MAKEFUN_OUTPUT_DIR=./out1 node --experimental-strip-types main.ts
MAKEFUN_OUTPUT_DIR=./out2 node --experimental-strip-types main.ts
cmp out1/entry.txt out2/entry.txt
```

Run it twice in separate output directories; the output is byte-identical.
