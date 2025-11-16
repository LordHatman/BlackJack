Blackjack – Browser Game (Version 1)

A lightweight browser-based Blackjack game written in HTML, CSS, and JavaScript.
The game features a full 52-card deck generated mathematically (no hard-coded cards), a functional hit/stay system, a dealer AI, and a small RPG-style progression element through configurable difficulty modes.

Features
✔ Full 52-card Deck (Mathematical Model)

Cards are represented as numbers 0–51.

Suit determined by index ranges (Hearts, Diamonds, Clubs, Spades).

Rank determined by index % 13.

Correct handling of Aces (1 or 11).

Image auto-mapping using "rank-suit" file naming.

✔ Blackjack Core Mechanics

Player receives two starting cards.

Dealer receives one shown card and one hidden (depending on difficulty).

Player actions: Hit or Stay.

Dealer acts according to Blackjack rules (hits until value ≥ 17).

Full round winner logic:

Blackjack

Bust

Higher hand wins

Push (tie)

Difficulty Settings

The game includes three difficulty modes, switchable in-game:

• Very Easy — Dealer Vision = 3

Dealer shows both cards and their total.

• Easy — Dealer Vision = 2

Dealer shows both cards, total hidden.

• Normal — Dealer Vision = 1 (Default)

Dealer shows only one card and hides the other.

Each setting directly updates:

dealerVision = 1 | 2 | 3

Point System (RPG-Lite)

Both Player and Dealer start at 100 points.

Win a round → +25 points

Lose a round → −25 points

Push → no points gained or lost

Match ends when:

Player reaches 0 points → GAME OVER

Player reaches 200 points → YOU WIN

Technical Notes

No frameworks, libraries, or external dependencies.

Card images follow naming pattern:

cards/{RANK}-{SUIT}.png


Example: A-S.png, 10-H.png, K-D.png.

Dealer’s card reveal logic controlled through dealerVision and forceRevealAll.

How to Run

Download the repository.

Ensure the /cards folder contains the correct card images.

Open index.html in any browser.

Play.
