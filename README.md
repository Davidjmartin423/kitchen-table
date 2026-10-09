# kitchen-table
1v1 battleground for Magic the Gathering Limited matches with friends!

# Cube Playtester

A two-player Magic: The Gathering table that runs in your browser, built for testing cube decks against a friend. It works like Moxfield's playtester, but with your opponent sitting across the table from you.

**▶ Play it here: https://YOUR-USERNAME.github.io/REPO-NAME/**

- No accounts or installs. Open the link, paste a decklist, and share a room code.
- The two browsers connect directly to each other (peer-to-peer over WebRTC).
- Card images come from [Scryfall](https://scryfall.com).
- Best-of-3 matches with sideboarding between games.
- Any number of 1v1 matches can run at once; each room code is its own private table.

---

## Getting started

1. **Open the link and enter your name.**
2. **One player clicks Host** and sends the 5-letter room code to their opponent (click the code at the top of the page to copy it). **The other player types it under Join.** Want to goldfish alone? Click **Practice solo**.
3. **Paste your decklist** and click **Load deck**. One card per line, like `1 Lightning Bolt`. Put your sideboard after a `Sideboard` line or after a blank line. Exports from Moxfield and MTGA, and the booster draft's **Copy list** button, all work, set codes included. Anything Scryfall can't find shows up as a plain text card.
4. **Both players click Ready.** Who goes first is random in game 1; after that, the loser of the previous game plays first. Everyone gets a London mulligan prompt.
5. **When a game ends,** either player clicks **End game…** and records the result. You'll both go to a sideboarding screen; click a card to move it between your deck and sideboard, then Ready up for the next game.

---

## Controls

### Mouse

| Do this | To |
|---|---|
| Click your library | Draw a card |
| Right-click your library | Draw X, scry, surveil, look at top X, mill, reveal, search, shuffle |
| Drag a card | Move it between hand, battlefield, library, graveyard, and exile |
| Double-click a permanent | Tap or untap it |
| Double-click a card in hand | Play it |
| Right-click any card | Counters, transform, face down, attach, copy, give control, move to any zone |
| Click / right-click a counter badge | Add or remove one counter |
| Hover any card | See it large in the preview panel |
| Right-click an opponent's permanent | Take control of it |
| Click opponent's graveyard or exile | Browse it |

### Keyboard

Press **?** in the app to see this list anytime.

| Key | Action | Key | Action |
|---|---|---|---|
| **D** | Draw (Shift+D: draw X) | **T** | Tap/untap hovered card |
| **U** | Untap all | **P** | Play hovered card from hand |
| **S** | Shuffle library | **F** | Transform hovered card |
| **N** | Create token | **Z** | Turn hovered card face down/up |
| **R** | Dice & coin | **C** | Copy hovered card as a token |
| **Y** | Tidy battlefield into rows | **A** | Attach hovered card to… |
| **+ / −** | +1/+1 counter on hovered card | **H / G / E** | Hovered card → hand / graveyard / exile |
| **Esc** | Close menus and dialogs | **O / B** | Hovered card → top / bottom of library |

### Sidebar

- **Life:** use the − and + buttons (Shift-click for ±5). Click your own total to type a number. You can adjust your opponent's life too.
- **Token:** search Scryfall for any token, or make a simple custom one.
- **Dice & coin:** results appear on both players' screens.
- **Hand…:** reveal your hand, discard at random, or shuffle your hand into your library.
- **A− / A+** (top bar): resize the cards to fit your screen.

---

## Good to know

- **Hidden information is on the honor system.** Your opponent's screen shows only how many cards are in your hand and library, but it isn't locked down against someone determined to peek.
- **Refreshing the page ends your game.** If the guest drops, they can rejoin the host's room with the same code and you can start a new game.
- **Can't connect?** Direct connections work on nearly all home networks. Strict work or school networks sometimes block them; try a different network.
- Your name, last decklist, and card size are remembered in your browser.

---

## Hosting your own copy

The whole app is a single file, `index.html`. To run your own copy:

1. Fork this repo, or create a new public repo and upload `index.html`.
2. Go to **Settings → Pages**, set the source to **Deploy from a branch**, choose **main** and **/ (root)**, and save.
3. After a minute or two, your copy is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

To update the site, upload a new `index.html` over the old one.

You can also just double-click `index.html` to open it locally. To try it with two players on one computer, open it in two tabs, host in one, and join from the other.

---

*Card images and data courtesy of [Scryfall](https://scryfall.com). Magic: The Gathering is © Wizards of the Coast. This is an unofficial fan project, not affiliated with or endorsed by Wizards of the Coast.*
