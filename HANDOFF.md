# HANDOFF — NightSkyEngine

**Last updated: 2026-11-22 (America/New_York).**
**Repo:** `mhvnsnt/NightSkyEngine` (PUBLIC), default branch `main`.
**Purpose of this file:** any agent that picks up work here reads this FIRST, then the linked docs. It states what we've done, where we're at, and what we're working toward — so the owner can say "go to this repo, pick up the work" and you just know. Update this file in the same PR whenever the state changes (add, don't delete).

## 1. What this repo is

Night Sky Engine — a free and open-source fighting game framework made in Unreal Engine 5. It is designed to be powerful yet easy to learn, and can be used to make 2D and 2.5D fighting games. It requires Unreal Engine 5.7. This branch targets higher-end machines (consoles, high-end PCs); a lower-fidelity branch exists upstream for weaker hardware.

At ~733 MB it is a full UE5 framework copy: `Source/`, `Content/`, `Plugins/`, `Config/`, `Platforms/`, `NightSkyEngine.uproject`. This is the owner's working copy of the framework, with his agent notes layered on (`AGENTS.md`, `WORKING-METHOD.md`, `docs/`). It is the fighting-game framework option next to Lyra (the general UE5 starter) — NightSkyEngine is the one built for fighters.

## 2. Where we're at

### DONE
- **Framework in place:** full NightSkyEngine UE5 project — source, content, plugins, config, platforms, project file. The README is the upstream framework README.
- **Anti-clobber laws merged (2026-10-17, PR #3):** the owner's anti-clobber laws are in `AGENTS.md`.
- **Working method stated (2026-10-27):** commits `8d95821` / `98f112f`, `WORKING-METHOD.md` at root.
- **Last push 2026-11-20** (repo metadata; no new content commits after Oct 27 — the push reflects repo-level activity).

### IN PROGRESS
- **Two open docs PRs (Nov 19–20, unmerged):** PR #6 — "Docs: pre-made parts first rule" (`docs/premade-parts-first`, 2026-11-20); PR #5 — "Docs: sourcing rule" (`docs/sourcing-rule`, 2026-11-19). Next step: a merge call on #5 and #6.
- **No fighter built on this framework is recorded in this repo.** Whether a game is being built from NightSkyEngine, which one, and what its first slice is, is NOT stated in the repo state read 2026-11-22. That is an open question (see §6), not hidden progress.

### BLOCKED
- **Nothing recorded as blocked in the repo state read 2026-11-22.** No blocked item is named in this repo. The open PRs are awaiting a merge decision, not unblocked work.
- **Engine requirement (not a block):** UE 5.7 is required. Do not open this project in an older engine version and expect it to work.

## 3. What we're working toward

**The goal:** a fighting-game framework the owner's fighters can actually be built on — 2D/2.5D, powerful yet easy to learn, running in UE 5.7 — kept faithful to upstream and understood well enough to build on.

**The bar (owner, general):** PULL-100% / REAL-SOURCE-ONLY — real code, wired in, never re-typed or hand-tooled. For a framework repo, done means: the copy is faithful to upstream, the owner's notes say how it is used, and a fighter built on it actually runs and plays.

**In order:** (1) merge or close PRs #5 and #6; (2) record which fighter/game builds from this framework and what its first slice is (owner's call); (3) keep the copy current with upstream NightSkyEngine releases.

## 4. Standing rules that apply here

- **Branch → PR → merge, always.** Never push to main directly. Add-only, zero-conflict PRs, no force pushes.
- **Checkpoint-and-save law:** CHECKPOINT.md first, update after every step; the repo is the save; resume, never restart.
- **No-temp-storage law:** nothing in /tmp or any wipeable location, ever. Everything goes straight into the repo or a durable folder the second it exists.
- **Real-source-only:** build from the real source. No hand-tooled lookalikes, no fake panels. Upstream framework stays faithful — local changes are layered and noted, not silent rewrites.
- **Anti-clobber law (owner 2026-10-17):** do not clobber other lanes' work. Add, don't overwrite. (Merged as PR #3.)
- **Licence-not-a-gate:** licence status never gates pulling in or using material that helps; licence/source is still logged honestly next to the item. (The framework is free and open source — its licence is in the repo; respect it as written.)
- **No-gaps / solve-it law:** a gap or block is never the end of the work — route-switch until it's done or every reasonable route is exhausted with exact errors recorded.

## 5. Key files and paths

| What | Where |
|---|---|
| Framework overview (upstream README) | `README.md` |
| Project file (UE 5.7 required) | `NightSkyEngine.uproject` |
| Source | `Source/` |
| Content | `Content/` |
| Plugins | `Plugins/` |
| Config / platforms | `Config/`, `Platforms/` |
| Agent notes / working method | `AGENTS.md`, `WORKING-METHOD.md` |
| Docs | `docs/` |
| Open PRs | #5 (sourcing rule), #6 (pre-made parts first rule) |
| Merged PR | #3 (anti-clobber laws, 2026-10-17) |

There are no releases in this repo. The lower-fidelity branch for weaker hardware is upstream — this branch targets higher-end machines.

## 6. Open decisions needing the owner

- **Merge PRs #5 and #6?** Two small docs-rule PRs open since Nov 19–20. Merging locks the rules in; leaving them open leaves the repo without the written rules. His call — lanes do not decide merges.
- **Which fighter/game builds from NightSkyEngine, and what's its first slice?** Not recorded in the repo. That is his call — a lane cannot pick a game for him. (Lyra is the other framework option; which one a given game uses is also his call.)
- **Keep tracking upstream NightSkyEngine releases?** Whether this copy tracks upstream or stays pinned is his call.
- **No other owner decision is recorded as open in this repo's state.**

## 7. How to pick up

1. Read this HANDOFF.md first, then `README.md`, `AGENTS.md`, and `WORKING-METHOD.md`.
2. Check the two open PRs (#5, #6) — leave them alone unless told to merge.
3. Do NOT start building a fighter on this framework until the owner says which game and what slice. This is the framework foundation; the game decision is his.
4. Open only in Unreal Engine 5.7 (per the README). If upstream-sync work is ordered, sync from upstream, keep local notes layered, and never silently rewrite upstream files.
5. Resume from the stated next step — never restart, never re-derive finished work.
6. Land work branch → PR → merge, add-only. Update this HANDOFF.md in the same PR when the state changes. Verify with your own eyes (a running build) before claiming anything done.
