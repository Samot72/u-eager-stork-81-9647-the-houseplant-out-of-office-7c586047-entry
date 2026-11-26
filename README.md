# The Houseplant Out-of-Office

[![Competition](https://make.fun/badge/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047.svg)](https://make.fun/c/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047)
[![Rank](https://make.fun/badge/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047/Samot72/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047-entry/rank.svg)](https://make.fun/c/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047)
[![Reward](https://make.fun/badge/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047/Samot72/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047-entry/reward.svg)](https://make.fun/c/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047)

Entry for [The Houseplant Out-of-Office](https://make.fun/c/u-eager-stork-81-9647-the-houseplant-out-of-office-7c586047)
— one out-of-office auto-reply, as if a houseplant had written it.

## The entry

> Thanks for your email. I'm a fern, ignored since March, thriving on spite. I'll reply when it rains indoors.

**108 characters** (code points; gate is 1–120, single line).

## How it works

`main.ts` (dependency-free, Node stdlib only) holds the line as a constant,
validates the gate — one line, 1–120 code points, not only whitespace — writes
it to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`), then reads the file
back and fails if the round trip does not match the entry exactly.

## Verify locally

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out node main.ts
cat /tmp/out/entry.txt
```

Expected output: `wrote 108-character entry to /tmp/out/entry.txt`, and
`entry.txt` contains exactly the line quoted above.

## License

MIT — see [LICENSE](LICENSE).
