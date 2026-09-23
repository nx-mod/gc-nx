# gc-nx

**GameCube games, running on your Switch.**

Not emulated. Each game is translated into a Switch program ahead of time and
runs natively, using your own disc for its files.

![](docs/images/launcher.png)

## What you need

- A Switch running homebrew
- A dump of a game you own, on the SD card
- A PC, once per game, to build it

## Getting started

1. Copy `gc-nx.nro` to `sdmc:/switch/`
2. Put your dump in `sdmc:/gc-nx/games/`
3. On a PC, run the builder once for that game — it reads your dump and produces
   the program that plays it
4. Open gc-nx on the Switch and pick the game

Full steps, with pictures: [docs/install.md](docs/install.md).

## What is here

| | |
|---|---|
| **Launcher** | the screen that lists what is on your card and starts it |
| **Examples** | a few games set up ready to build, and homebrew that runs as it is |

## Games

Each game is its own small project holding nothing but what that game needs —
never the game itself. Browse them in [examples](examples).

## Homebrew

GameCube homebrew runs here too, and unlike games it can be handed out already
built, because it contains nothing Nintendo made. A few are included as
examples.

## Questions

**Is this legal?** Your dump stays on your machine and nothing of Nintendo's is
distributed. You build from a disc you own.

**Will my game work?** Only the ones listed. Adding one is work, not a setting.

**Do I need a PC?** Once per game, to build it. Playing does not.

## For developers

The machinery lives elsewhere: [gccompiled-nx](https://github.com/nx-mod/gccompiled-nx)
turns a disc into a program, [libgc-nx](https://github.com/nx-mod/libgc-nx) is
the GameCube's hardware as a library, and
[libdol-nx](https://github.com/nx-mod/libdol-nx) is everything the GameCube and
the Wii share.

## License

GPL-3.0-or-later. No game code or data is included or distributed.
