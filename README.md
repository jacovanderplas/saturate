# Saturate

A real-time strategy game about spreading color. You and two bots each start with one marker on a dark board scattered with resources. Markers spread their color. Every resource in your color pays you points each second, and you spend those points on new markers and upgrades.

**Play it:** https://jacovanderplas.github.io/saturate/

## How a match works

1. Each player places one marker, in random order.
2. The clock starts. Markers spread their color outward, and overlapping colors fight for the ground.
3. Every resource you color pays you points. A contested resource splits its payout.
4. Spend points on new markers (inside your own color, or anywhere if you turn that rule off) or on upgrades:
   - **Strength** pushes your color harder.
   - **Reach** spreads it further.
   - **Hold** makes the marker harder to capture.
5. When enemy color outweighs a marker's own Strength and Hold, the marker drains and switches sides. Captures start 45 seconds in.
6. Most points earned when time runs out wins. Cover the whole board in your color and you win at once.

## Controls

- Click or tap a glowing **+** inside your color to place a marker.
- Click or tap one of your markers to open its three upgrade buttons.
- Keyboard: `1` `2` `3` upgrade the open marker, `Space` pauses, `Esc` closes the menu.
- On a phone, a match fills the screen sideways. Hold the phone sideways, even if its screen doesn't rotate: the game turns the view itself when the screen stays upright. Time, points and standings sit beside the board, with Pause and Exit buttons.

## Bots

| Level | How they play |
|---|---|
| Easy | Slow and careless. They earn about half as much and don't hunt your markers. |
| Normal | Steady. They earn a bit less than you and would rather fight each other. |
| Hard | Quick and sharp. They earn as much as you and come for your markers. |

## Running it

It's a single `index.html` with no build step. Open it in a browser, or serve the folder with any static server. Fonts load from Google Fonts. Without a connection the game falls back to system fonts.
