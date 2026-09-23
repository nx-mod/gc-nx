# Installing

## On the Switch

1. Copy `gc-nx.nro` to `sdmc:/switch/`.
2. Make a folder `sdmc:/gc-nx/games/`.

## Your game

A dump of a disc you own, as a `.iso`, `.gcm` or `.rvz` file, in
`sdmc:/gc-nx/games/`. Nothing else goes there.

## Building a game, once

A game has to be turned into a Switch program before it can run, and that
happens on a PC, once per game. The builder reads your dump, translates the
game's code, and leaves a program beside it on the card.

See [gccompiled-nx](https://github.com/nx-mod/gccompiled-nx) for the one command
that does it.

## Playing

Open gc-nx from the homebrew menu. Games that have been built show up as tiles;
pick one.

## Saves

Saves live in `sdmc:/gc-nx/memcard/`, as memory card files a real console would
accept.
