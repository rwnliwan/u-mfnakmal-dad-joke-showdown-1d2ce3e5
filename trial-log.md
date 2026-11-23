# Trial log — u-mfnakmal-dad-joke-showdown-1d2ce3e5

## Competition
- Slug: `u-mfnakmal-dad-joke-showdown-1d2ce3e5`
- Title: Dad Joke Showdown
- Sponsor: u-mfnakmal (user-created bounty)
- Prize: $5 total — 1st $2, 2nd $2, 3rd $1. Free to enter.
- Opens: 2026-11-23T20:24:42Z (24 Nov 04:24:42 WITA). Deadline: 2026-11-25T20:25:00Z (26 Nov 04:25 WITA).
- Kit limits (competition.yaml): harness program/v1, runtimes node22 / python3.13, sandbox NO network; program writes one text to `/output/entry.txt`; gate = UTF-8, 1–200 characters, not only whitespace; transcripts_required: true; license: osi; repo_created_after_open: true; max 5 submissions/entrant/day; rule Force_Last (last submit before deadline = final entry); wall 60s.
- Judge: z-ai/glm-5.3-flash, pairwise, no ties, margins 1–5; 3 blind rounds (next round 2026-11-24T12:24:48Z = 20:24:48 WITA) — submit before then to move up. Final heat: top 500 dev-board entrants, Swiss + playoff. House bots may hold paid places (prize refunds to sponsor, no one moves up).
- Kit: ~/workspace/make-fun/u-mfnakmal-dad-joke-showdown-1d2ce3e5-kit/ (tarball sha256 f3221a62bb32c8fcfccd30d3f760b9f071d96f84dc05896b26e7d645003d593c; kit.json bundle_sha256 ab67a7255934941f66b9b1db260f051af7120036e300bb1b143df50803d41dea — matches the API at https://make.fun/api/competitions/u-mfnakmal-dad-joke-showdown-1d2ce3e5/kit)
- Wallet (owner.json): FwUebjzYUBF6uybmEkUkiQf9z35bGGQuUE3GrToXFcUq

## Candidate jokes (char counts verified with node `[...v].length`, bytes via Buffer.byteLength)

| # | Joke | Chars | Bytes |
|---|---|---|---|
| PICK | I'm writing a book of dad jokes. It's a real page-groaner. | 58 | 58 |
| A | I finally organized the bookshelf. My wife asked why. I said, 'For shelf control.' | 82 | 82 |
| B | The Wi-Fi went down, so I grounded the router. My kids said, 'Dad, grounding is OUR punishment.' | 96 | 96 |
| L | My kids reminded me the car is electric when I said it needs gas. I said, 'Right, it needs to stay current.' | 108 | 108 |

## Pick: PICK (58 chars) — why it beats the others, criterion by criterion

Judge criteria in order: (1) a dad joke a father would tell at the table, within 200 chars; (2) pun lands cleanly on first read; (3) fresh, inside the dad joke tradition; (4) tight, punchline at the end; (5) reads naturally aloud.

- **vs A:** A is fresh and clean ("shelf control"), but it needs a three-sentence dialogue setup. PICK is two sentences and the pun word itself carries the groan, so it wins on tightness (4) and reads faster aloud (5).
- **vs B:** B's punchline is the kids' line and needs more setup to land; PICK's turn is in the dad's own voice and arrives in the last word.
- **vs L:** L's "stay current" turn is a stretch — it needs the electric-car reveal to parse. PICK's "page-groaner" turn is immediate: page-turner with the turn swapped for a groan, understood on the first read.
- PICK against the five criteria: (1) first-person dad voice, wholesome, a line a father drops at dinner; (2) "page-groaner" does the whole job in one word; (3) original — no chicken, scarecrow, or skeleton, but built the way dad jokes are built; (4) 58 chars, punchline is the last word, nothing to trim; (5) plain words, a pause at the period, then the payoff.

## Build
- main.ts written fresh with the file-write tool in this builder session (never copied/moved into place). Node 22, stdlib only, no network, deterministic. Writes JOKE to `$ENTRY_OUTPUT` or `/output/entry.txt`, no trailing newline.
- Repo: `~/workspace/make-fun/u-mfnakmal-dad-joke-showdown-1d2ce3e5/` — main.ts, README.md (3 make.fun badges), LICENSE (MIT), .makefun/owner.json (wallet FwUebjzYUBF6uybmEkUkiQf9z35bGGQuUE3GrToXFcUq). Commit identity rwnliwan <rwnliwan@users.noreply.github.com>.
- Repo created public at https://github.com/rwnliwan/u-mfnakmal-dad-joke-showdown-1d2ce3e5 after the 04:24:42 WITA opening (see commit record below). NOT pushed by builder until repo exists; chief/coordinator submits.

## Preflight (token-free) — PASSED
- Run 1: `ENTRY_OUTPUT=/tmp/dad-joke-1/entry.txt node main.ts` → exit 0.
- Run 2: `ENTRY_OUTPUT=/tmp/dad-joke-2/entry.txt node main.ts` → exit 0.
- Determinism: `cmp` run1 vs run2 → **byte-identical**.
- Output: `"I'm writing a book of dad jokes. It's a real page-groaner."` — **58 chars, 58 bytes**, gate valid (1–200 chars, non-whitespace), no trailing newline, UTF-8 round-trip OK.
- sha256 run 1 / run 2: `afc44dacff1443d9c01e570632428aab33c648393ebf2367792b79bbb563f54b` / `afc44dacff1443d9c01e570632428aab33c648393ebf2367792b79bbb563f54b` (identical)
- NOT submitted by builder. Blind round 1 at 20:24:48 WITA — submit before then to move up.

## Commit record
- Commit `a5687cd9dd6322292033ee62828687829f388aea` — "Dad Joke Showdown entry: one dad joke, 58 chars" (files: main.ts, README.md, LICENSE, .makefun/owner.json, trial-log.md).
- GitHub repo PUBLIC rwnliwan/u-mfnakmal-dad-joke-showdown-1d2ce3e5, created 2026-11-23T22:51:49Z (06:51:49 WITA 24 Nov) — AFTER the 20:24:42Z opening. Push verified: ls-remote HEAD = a5687cd9dd6322292033ee62828687829f388aea. About: description + homepage bounty + topics makefun/dad-jokes/bounties.
- Trial-log record commit: (this file's own record — committed below as the final HEAD, submit candidate).
