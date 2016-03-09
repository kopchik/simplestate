# simplestate
Saltstack knockoff: simple, pythonic, free of yaml warts, does not gets in the way

## Why not saltstack

While salt has many interesting ideas it's also a big source of frustation:
http://stevebennett.me/2014/02/17/one-week-of-salt-frustrations-and-reflections/

I think simple things should be done in a simple way.
The tool must help achieving the goal, not to dictate what are the goals and how to get there.


## How it works

The "configuration" file (really a python script) describes the [workflow graph](https://en.wikipedia.org/wiki/Flowchart).
Then the user just executes it. The graph is traversed according to the dependencies. Every dependency executes some code and.. voila!
It is that simple, nothing else is done. No side effects, not tricky software dependencies and no magic under the hood.
The script defines the whole process.

## Goals

1. Keep it simple
2. Easy to use for newcommers
3. Meaningful diagnostic messages
4. Expendable
5. Minimum software dependencies
