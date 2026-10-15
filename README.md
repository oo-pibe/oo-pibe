# oo-pibe

## review-seal

Commits of covered files wait until a separate Claude session has reviewed the current version against a checklist. Reviews can expire and get re-checked on a schedule. Built for docs and go-to-market content kept in git: outreach sequences, battlecards, blog posts. Claude Code plugin, git hook and GitHub Action.

[repo](https://github.com/oo-pibe/review-seal) · [npm](https://www.npmjs.com/package/review-seal)

## audio-bed-check

If you render videos from a script, the background audio gets assembled by code and nobody listens to every file. This checks the rendered file for the three things that go wrong: the background clip was repeated to fill the time, the level jumps where two recordings were joined, or the voiceover is mixed too close to the background to be heard. It exits non-zero when it finds one, so it can sit in a build. Python, ffmpeg.

[repo](https://github.com/oo-pibe/audio-bed-check) · [PyPI](https://pypi.org/project/audio-bed-check/) · listed in [Remotion's tooling docs](https://www.remotion.dev/docs/resources)

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. Built after geo-tz couldn't find its data files in a serverless function and the lightweight alternative was an hour off at a border town. Also added to timezone-boundary-builder's list of lookup libraries.

[repo](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)
