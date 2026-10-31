# MPC VST · field notes

Working notes on building native VST2 plugins for MPC OS and Force — what actually works, what it
costs, and where the traps are. Written from the bench: every number was measured on an MPC Live II
(MPC OS 3.9.1.2), and the places where something is still unproven say so.

**Site:** https://mitchoster.github.io/mpc-vst-dev-guide/

## Pages

| page | what |
|---|---|
| `index.html` | what a plugin is, the loop, where to start |
| `start.html` | toolchain, the five files that matter, the four commands, build traps, cost |
| `device.html` | fourteen facts that cost time: services, paths, skins, `/proc`, crashes |
| `screen.html` | the companion screen: giving a plugin a real UI without asking MPC to draw it |
| `test.html` | the testing ladder and the bug each rung caught |
| `ship.html` | release, licence, export, catalog PR, the socket warning |
| `agents.html` | what exists for agent-driven development, what is missing, what not to build |

## What this is not

Not a framework. The framework is [sd88me/mpc-vst-plugins](https://github.com/sd88me/mpc-vst-plugins)
(MIT) — wrapper, parameter compiler, skin generator, host test, bench, packager, catalog. These notes
pick up after “it builds”.

The worked example behind every page is
[MPC Multihead Echo](https://github.com/mitchoster/mpc-vst-multihead-echo) (GPL-3.0).

## Credit

The companion-screen idea is [VADER](https://github.com/sunskiefer/VADER)’s (sunskiefer / L’Cronx,
MIT, since v0.6.0 2026-10-24). Nothing else here is borrowed.

No Akai or AIR assets, text or code. Product names are used descriptively.

Text: MIT.
