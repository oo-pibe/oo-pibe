# oo-pibe

I run [Road to Kickoff](https://roadtokickoff.com), a football trip planner, and write the code behind it: the fixture and kickoff-time pipeline, the checks on whether a kickoff time can be trusted yet, and the tooling that turns match data into guides and social posts. 

Mostly TypeScript, some Python. A lot of it is closer to go-to-market engineering than product work: harvesters, content pipelines, review gates. Most of it gets written with Claude Code these days.

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. Extracted from Road to Kickoff after geo-tz couldn't find its data files in a serverless function and the lightweight alternative was an hour off at a border town. On npm; ships a skill so coding agents can use it without reading the source.

[repo](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)

Contact: contact@roadtokickoff.com
