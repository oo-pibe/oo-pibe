# oo-pibe

I build small tools when something I'm using gets in the way. Mostly TypeScript, mostly for code that runs in a build step or on a server.

## tz-at-point

Exact IANA timezones for a fixed list of coordinates, resolved at build time so nothing is read at runtime. I wrote it after geo-tz couldn't find its data files inside a serverless function and the lightweight alternative put a Finnish border town in the Swedish timezone. It's on npm with provenance, and it ships a skill so coding agents can use it without reading the source.

[github.com/oo-pibe/tz-at-point](https://github.com/oo-pibe/tz-at-point) · [npm](https://www.npmjs.com/package/tz-at-point)

## How I work

I'd rather ship one thing that has been attacked properly than three that pass their own tests. Before tz-at-point went public it was fuzzed against geo-tz over millions of points, mutation-tested, and put through independent review. The docs say what it doesn't do as plainly as what it does.

Contact: contact@roadtokickoff.com
