# oo-pibe

I run [Road to Kickoff](https://roadtokickoff.com), a football trip planner, and write the code behind it: the fixture and kickoff-time pipeline, the checks on whether a kickoff time can be trusted yet, and the tooling that turns match data into guides and social posts. 

Mostly TypeScript, some Python. A lot of it is closer to go-to-market engineering than product work: harvesters, content pipelines, review gates. Most of it gets written with Claude Code these days.

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. Extracted from Road to Kickoff after geo-tz couldn't find its data files in a serverless function and the lightweight alternative was an hour off at a border town. On npm; ships a skill so coding agents can use it without reading the source.

[repo](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)

## audio-bed-check

Three checks on a rendered audio bed or a voiceover mix: does the bed repeat itself, does its level jump at a join, does the voice sit far enough above it. Came out of the same video pipeline after a bed with a 7 dB join got past every automated check and was caught by ear. Python, ffmpeg, BS.1770 loudness in numpy; ships a skill too.

[repo](https://github.com/oo-pibe/audio-bed-check) · [PyPI](https://pypi.org/project/audio-bed-check/)

Contact: contact@roadtokickoff.com
