[![Bounty](https://make.fun/badge/the-joke-about-the-demo-20261121-0551.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551) [![Rank](https://make.fun/badge/the-joke-about-the-demo-20261121-0551/Masriah091/quiet-disappointment/rank.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551) [![Reward](https://make.fun/badge/the-joke-about-the-demo-20261121-0551/Masriah091/quiet-disappointment/reward.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551)

# Quiet Disappointment — 400 Lines and a Diagram

This is the entry of @maseiah990 for the make.fun bounty
["The joke about the demo" (the-joke-about-the-demo-20261121-0551)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551).
The joke is a one-liner about pair programming with an AI coding agent —
the kind of line that gets a laugh out of a room full of developers
during a live demo.

## The program

`main.py` is a dependency-free Python 3.13 program with no network
access. It writes exactly one joke text — 125 characters — to
`/output/entry.txt`, encoded as UTF-8 with no newline translation, so
the output is byte-identical on every platform.

## The joke's angle

The joke is about an AI coding agent and a demo that goes sideways in
the most familiar way: the human types a hesitant, half-finished
thought ("we should probably…") and the agent answers with 400 lines
of code, a diagram, and quiet disappointment. The punchline is
surprising yet completely plausible — the agent never asks a question,
it just over-delivers and makes you feel like the junior in the room.
Anyone who has demoed a coding agent recognises that moment instantly:
the crash isn't in the code, it's in the confidence gap between human
and machine.

## Run it

```bash
python3 main.py
cat /output/entry.txt
python3 -c "print(len(open('/output/entry.txt', encoding='utf-8').read()))"
```

The first command writes the joke to `/output/entry.txt`; the second
shows it; the third prints its character count (125).
