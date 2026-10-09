# oo-pibe

I run [Road to Kickoff](https://roadtokickoff.com), a football trip planner, and write the code behind it: the fixture and kickoff-time pipeline, the checks on whether a kickoff time can be trusted yet, and the tooling that turns match data into guides and social posts. 

Mostly TypeScript, some Python. A lot of it is closer to go-to-market engineering than product work: harvesters, content pipelines, review gates.

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. Extracted after geo-tz couldn't find its data files in a serverless function and the lightweight alternative was an hour off at a border town. 

[repo](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)

## audio-bed-check

If you render videos from a script, the background audio gets assembled by code and nobody listens to every file. This checks the rendered file for the three things that go wrong: the background clip was repeated to fill the time, the level jumps where two recordings were joined, or the voiceover is mixed too close to the background to be heard without effort. It exits non-zero when it finds one, so it can sit in a build. Python, ffmpeg; ships a skill too.

[repo](https://github.com/oo-pibe/audio-bed-check) · [PyPI](https://pypi.org/project/audio-bed-check/) · listed in [Remotion's tooling docs](https://www.remotion.dev/docs/resources)
