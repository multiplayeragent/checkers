# Checkers

Jump, chain the jumps, get crowned. A multiplayer starter game from [Multiplayer Agent](https://multiplayeragent.com): 2D, turn-based, 2 players plus anyone who wants to watch, with a bot that takes any empty seat.

![Checkers](poster.jpg)

## How it plays

Classic 8×8 checkers: move diagonally, jump to capture (jumps are forced, and you keep jumping while you can), and reach the far side to become a king that moves both ways. The first two players take the seats; anyone else watches. Alone? A bot plays the other side, and a friend who joins takes over from it.

**Controls:** Click or tap a piece, then a dot (or drag it there).

## Make it yours in the Game Builder

Open the [Game Builder](https://multiplayeragent.com), choose **Start from a starter game** and pick Checkers. It opens as version 1 in your studio, ready to play and publish. Then ask for changes, for example:

- Let kings fly any distance along a diagonal
- Add a 20-second timer for each move
- Make it a candy board with gummy pieces

## Run it yourself

1. Get a free publishable key (`pk_…`) at [multiplayeragent.com](https://multiplayeragent.com).
2. In `index.html`, put it in place of `pk_REPLACE_ME` in the `MP_CONNECT` block.
3. Open `index.html` in a browser. No build step and no server needed.

Without a key it still runs, offline against the bot.

## How it is built

- One `index.html`. The comment at the top of the script maps the code and explains the multiplayer.
- **Host-run rules:** The host's browser checks every move; if it leaves, the next player takes over.
- **Bots:** A bot takes any empty seat, so you can play alone, and a friend who joins takes the bot's side.
- **Live sync:** Players and watchers see the same board, every hop and capture animated.
- **Leaderboard:** Most wins, shown after every game.
- `?attract` runs it offline, bot against bot. The preview video is recorded from it.

## License

MIT.
