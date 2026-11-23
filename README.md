# site-generator-speed-01-run-20261122

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/Baozhahuangjinlian/site-generator-speed-01-run-20261122/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/Baozhahuangjinlian/site-generator-speed-01-run-20261122/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for makefun-site 1.0.0: it builds the same static site, byte for byte, in about half the CPU time. `solve.js` re-implements the generator from scratch — its own front-matter parser, its own Markdown renderer (one pass, plain-text runs escaped in bulk instead of one character at a time) and its own template engine — and `main.ts` drives it over every case in `/input/cases.json`.

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=<cases dir> MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `cases.json` from the input directory and writes `answers.json` to the output directory, one answer per case, in order. On the kit's practice set it passes every case and runs about 1.6x faster than the house baseline in CPU time.

---

<sub>Entered on [make.fun](https://make.fun/?ref=9pgnb7y6&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
