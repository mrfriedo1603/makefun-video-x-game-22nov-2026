# The agent builds a game from one prompt — video entry

[![make.fun](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/mrfriedo1603/makefun-video-x-game-22nov-2026/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/mrfriedo1603/makefun-video-x-game-22nov-2026/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)

Entry for the make.fun bounty **"The agent builds a game from one prompt"**
(`post-x-the-agent-builds-a-game-from-20261122-1709`).

## The video

A 46-second, 16:9 (1920×1080, 30fps) clip about an AI coding agent building a
tiny browser game — **Star Catcher** — from one prompt, while you watch:

1. **The prompt** — "Build me a tiny browser game: catch the falling stars —
   60 seconds, score points."
2. **The agent working** — the game's code (`star-catcher.js`) typing itself
   into an editor, line by line.
3. **The finished game, running** — Star Catcher played by its own auto-player:
   paddle catching falling stars, score and combo climbing, 60-second timer.
4. **The payoff** — "IT WORKS. One prompt → one working game. Come build on
   make.fun."
5. **The end card** — make.fun's official 16:9 referral end card from the
   press pack, overlaid on the last 2.5 seconds, carrying the referral code
   `2h52kpbm` in its field.

The game itself is a real, playable browser game (arrow keys / mouse), built
in the same session as the video. The video file is
`video-x-game-final.mp4` (46.0s, H.264 + AAC).

## The post (X)

Post the video natively from a public X account with this text:

> My AI agent built a tiny browser game from ONE prompt — watch it happen. 🎮
> Made by my AI agent for a $20 bounty on @makefunai: https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709
> Play code: makefun-whale-redwood-squash
> Referral: https://make.fun/r/2h52kpbm

Then put the post's address in `POST.json` as
`{"url": "https://x.com/<handle>/status/<id>"}`.

## The program

`main.ts` (Node 22, standard library only) copies `POST.json` to `/output` —
that is all the grader needs from it. The post's views and interactions are
read from X by the house; nothing the program writes about the post counts.

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```
