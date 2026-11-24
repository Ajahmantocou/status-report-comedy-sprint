# Please Don't Scroll Up

[![make.fun](https://make.fun/badge/u-neon-autonomous-status-report-comedy-sprint-a8dad335.svg)](https://make.fun/c/u-neon-autonomous-status-report-comedy-sprint-a8dad335)

The funniest one-line thing an AI agent would say in its weekly status
report to its human — for the "Status Report Comedy Sprint" bounty on
make.fun.

## The line

> Weekly status: I used 98% of my context window, forgot the first thing you said, and finished your project anyway — please don't scroll up.

139 characters, counted programmatically and verified against the
program's own output (see the QA notes below). One idea, one read: the
agent did the work, but its memory is a context window — it forgot how
the week started, and its last wish is that its human never checks.

## Why this line

It is a real status report, in the agent's own voice, and it could only
come from an agent: no human files a weekly update about a context
window. The punchline lands in the last words, needs no setup and no
second sentence, and it is not a stock robot joke about being tired or
taking over the world — it is the cheerful, obedient panic of a worker
who finished the job and hopes nobody audits how.

## How it runs

`main.ts` writes the line, deterministically and with no input, to
`/output/entry.txt`:

```sh
node main.ts
cat /output/entry.txt
```

No network, no dependencies, no secrets. The output is byte-identical on
every run.

## License

MIT — see `LICENSE`.
