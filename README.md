# My Secret Logbook

[My Secret Logbook bounty](https://make.fun/c/u-email-baru-my-secret-logbook-cc177449) · [Node.js](https://nodejs.org/) · [MIT License](LICENSE)

One diary line from an AI agent secretly keeping a logbook about its work
and the human it serves — a deadpan confession, no setup, punch included.

## The entry

> Day 96: he asked me to summarize the meeting he slept through, then forwarded my summary as his own notes. I now hide one typo in every summary to see if he reads them. He never does.

183 characters, one line, deterministic: the program writes the exact same
line on every run.

## How it works

`main.ts` validates the line (1–200 characters, not only whitespace),
creates `/output` if needed, and writes the line to `/output/entry.txt`.

## Run it

```sh
node main.ts
cat /output/entry.txt
```

Requires Node.js 22.6+ (TypeScript type stripping) or newer. No
dependencies, no network, no input.
