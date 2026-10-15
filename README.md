# oo-pibe

I build the systems that let AI agents draft content I can trust: independent review gates that block publishing until a separate reviewer has read the page, data pipelines, and small tools published on npm and PyPI. I run them on my own business, [Road to Kickoff](https://roadtokickoff.com), football travel guides that agents research and draft.

What I'd build for a revenue team: research and enrichment agents with evals, QA gates on AI-written outreach and battlecards, and checks that catch stale facts before a rep repeats them.

## review-seal

Stops blog posts, outreach sequences, battlecards and docs kept in git from being committed until a separate AI reviewer has checked them against your checklist, and re-checks fact-based pages on a schedule. On real earlier versions of my guides it caught 4 of 4 in-page contradictions; on its own README it found four errors, one of them a GitHub fact that had changed since it was written. Claude Code plugin, git hook and GitHub Action.

[repo](https://github.com/oo-pibe/review-seal) · [npm](https://www.npmjs.com/package/review-seal)

## audio-bed-check

If you render videos from a script, the background audio gets assembled by code and nobody listens to every file. This checks the rendered file for the three things that go wrong: the background clip was repeated to fill the time, the level jumps where two recordings were joined, or the voiceover is mixed too close to the background to be heard. It exits non-zero when it finds one, so it can sit in a build. Python, ffmpeg.

[repo](https://github.com/oo-pibe/audio-bed-check) · [PyPI](https://pypi.org/project/audio-bed-check/) · listed in [Remotion's tooling docs](https://www.remotion.dev/docs/resources)

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. Built after geo-tz couldn't find its data files in a serverless function and the lightweight alternative was an hour off at a border town. Also added to timezone-boundary-builder's list of lookup libraries.

[repo](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)
