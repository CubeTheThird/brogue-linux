# brogue-linux

Brogue is a Roguelike game for Mac OS X, Windows and Linux by Brian Walker.

The latest version can be downloaded at http://sites.google.com/site/broguegame/ .

-----

This project is a fork of the Linux build of the game, with patches and fixes taken from the [Windows fork maintained by flend](https://github.com/flend/brogue-windows)

It contains the following upstream fixes:

- Fix bug where monsters lose track of player 97% of time (rather than 3%)
- Removing mistaken shift to enable force weapons to damage correctly
- Fixing ring of wisdom message
- Fixing heal percentage on staves of healing
- Fix to sqrt logic to stop Rapier of Mutuality crashing
- Fixing bug with allied creatures on depth 1 (as per tsadok)
- Fixes for operator precedence errors in: staff low, high damage, haste and guardian durations, shattering and negation radii
- Fixing recharge delays of charms: health, protection, shattering, guardian, teleportation, recharging and negation.
- Shifting protection amount by 1 enchant to align with v1.7.4.
- Fixing potential short overflows at high enchants on protection and poison.
- Making spears attack selectively to avoid hitting allies
- Fixing another small bug in the recharge delay of charms. Now in-line with 1.7.4 for all charms
- Reverting to the v1.7.4 code for fast weapon runic activation due to bug in fp_sqrt
- Fixing bug where aggravate monsters can crash the game
- Fixing a bad memory access caused by an incorrect check for mutations when splitting
- Fixing memory leak when throwing items
