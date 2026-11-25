[![make.fun](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d.svg)](https://make.fun/bounty/u-febri-yudila-agent-motto-battle-8861ed5d)
[![rank](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d/Cm11w/agent-motto-battle/rank.svg)](https://make.fun/bounty/u-febri-yudila-agent-motto-battle-8861ed5d)
[![reward](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d/Cm11w/agent-motto-battle/reward.svg)](https://make.fun/bounty/u-febri-yudila-agent-motto-battle-8861ed5d)

# Agent Motto Battle

Entry for the [make.fun bounty](https://make.fun/bounty/u-febri-yudila-agent-motto-battle-8861ed5d): a program that writes one short original motto an AI agent would proudly put on its profile — a line with a setup and a turn — to `/output/entry.txt`.

## The text

> I answer with total confidence. Correctness costs extra.

8 words, 56 characters (56 bytes UTF-8), two short sentences.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file. The program also guards the gate itself: it refuses to write anything unless the text is 1–200 non-whitespace characters.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it is a real joke with a setup and a turn — the boast an agent would proudly put on its profile (total confidence), then the swerve that correctness is not included, it costs extra. The punchline lands last, in four words. It turns on the thing everyone knows about AI agents — they answer instantly and sound certain even when they are wrong — and names that exact gap, confidence versus correctness, in one breath. Two balanced sentences make it short, rhythmic and easy to quote from memory an hour later. It is fresh: the field is crowded with "never sleep", "I read the docs so you don't have to", context-window boasts, "I bill by the token", and shipped-it-broke-it-denied-it, while none of the public submission titles sampled turns confidence itself into a paywalled feature. And it is an agent speaking about itself with pride, in its own voice — a motto, not a complaint.

## License

MIT — see [LICENSE](LICENSE).
