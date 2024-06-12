# Pixel Casino

## Overview

**Pixel Casino** is a free downloadable casino game that allows you to enjoy multiplayer Blackjack and Baccarat with up to five players. Players can choose to join private or public lobbies. All players start with 500 currency and can increase their wealth through gameplay. 

### Game Features

- **Multiplayer Blackjack and Baccarat:** Play with up to five players in both public and private lobbies.
- **Starting Balance:** Every player begins with 500 currency.
- **Blackjack Rules:**
  - Dealer stands on all 17s.
  - Blackjack pays 3 to 2.
  - Infinite Splits
  - The deck is made of 6 decks and is shuffled after 3/4 of the cards have been played.
  - Cards are dealt unbiased and at random, simulating a real deck.
  - Dealer always checks for blackjack before play starts and Insurance pays 2 to 1.
  - Minimum bet is 1$
- **Baccarat Rules**
  - Place bets on the Banker Hand, Player Hand, Tie, or Pair.
  - Banker Bet pays 19 to 20 and Player Bet pays 1 to 1
  - Pair Bet pays 11 to 1 and Tie Bet pays 8 to 1
  - Card drawing follows typical casino baccarat rules
  - Minimum Bet is 1$

## Installation

To install and play **Pixel Casino**, follow these steps:

1. **Download the Game:**
   - Download the zip folder named `PixelCasino.zip` from the release page, this is the newest version as old versions may no longer be supported (but are available in the `Old Versions` folder).

2. **Extract the Game:**
   - Unzip the `PixelCasinoV#.#.zip` folder to a location of your choice on your computer.
   - Do not remove any files or folders from the unzipped folder.

3. **Run the Game:**
   - Navigate to the unzipped folder and run the executable file to start the game.

## Getting Started

1. **Launching the Game:**
   - Double-click the executable file to launch **Pixel Casino**.

2. **Sign Up or Log In**
   - Log in to your account or sign up through the signup page.

3. **Choose Game**
   - Choose from our available casino games, either BlackJack or Baccarat. (More games coming soon)
   - You can also access the Options menu from here and change your username
   
4. **Joining a Lobby:**
   - Select whether you want to join a public or private lobby.
   - To join a random public game simply click on **Public Lobby** and let the fun begin.
   - To start a new private lobby leave the lobby id box blank. Else to join a private lobby enter the lobby ID for the lobby you wish to join.

5. **Gameplay:**
   - **Blackjack:**
     - Play classic Blackjack with Pixel Graphics according to the rules outlined in the game features section.
   - **Baccarat**
     - Play the classic casino game Baccarat Rules outlined above. 
   - **Craps:**
     - Enjoy a classic game of Craps with your friends or other online players. **COMING SOON**
   - **Poker**
     - Play Texas Holdem Poker against others or friends online. **COMING SOON**

## System Requirements
- **Storage:** 121 MB available space

## Contributing
We welcome contributions to improve **Pixel Casino**. If you would like to contribute, please reach out to the owner of the repository.

## Do Not Distribute or Copy. 
## Do Not Sell as Own Product

Enjoy playing **Pixel Casino**!

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Update History

### Version 1.3

#### New Game Mode: Baccarat
- **Baccarat**: A brand new game mode, Baccarat, has been added. Up to five players can play together, following all regular casino rules. Players can select a chip type and click on the felt to place their bets.

#### Server-Side Additions
- **Baccarat Server Implementation**: Implemented all necessary server-side additions for Baccarat.

#### Client-Side Additions and Visuals
- **Baccarat Client Implementation**: Began client-side changes to incorporate Baccarat into the game.
- **Baccarat Visuals**: Set up Baccarat visuals, allowing players to bet by selecting a chip type and clicking on the felt where they want to place their money.

#### Feature Enhancements
- **Blackjack Dealer Blackjack Fix**: Ensured all players see the flipped cards when the dealer has blackjack by checking that all players have communicated with the server before flipping a new card.
- **Blackjack Insurance Fix**: Modified Blackjack insurance to prompt all players simultaneously, rather than procedurally.

#### Bug Fixes and Improvements
- **Baccarat Betting System**: Fixed issues where more than one chip could be placed on a bet with a single click. Removed unnecessary delays when placing a bet and added bet displays for other players.
- **Baccarat Gameplay**: Resolved issues with dealing extra cards in multiplayer mode and fixed the bug that allowed players to mess with bets after pressing deal. Finalized Baccarat gameplay to ensure proper multiplayer functionality.
- **Ready Status Display**: Added "Ready" or "Not Ready" display above players to show who is ready for the cards to be dealt. 
- **Hand Value Display**: Added text below the player and banker hands to display hand values, easing gameplay.
- **Server Logic and Betting System Fixes**: Made several changes to server logic and draw card logic to reflect true Baccarat rules. Fixed the betting system to prevent players from betting more than their account balance.
- **UI Improvements**: Fixed positions of other players' bets on the screen and evenly spaced out all bet boards for improved game aesthetics.

We are thrilled to bring you this new update and hope you enjoy the new Baccarat game mode along with the improvements to the overall game experience. Thank you for playing Pixel Casino and for your continued support!

## Version 1.2 Update
 
We are excited to announce the release of version 1.2 of **Pixel Casino**! This update brings several significant improvements and bug fixes, enhancing your gaming experience and preparing the codebase for future expansions. Below is a detailed overview of the changes included in this release.

### What's New in Version 1.2

#### Efficiency Improvements and Bug Fixes
- **Efficiency Enhancements**: Various functions have been optimized for better performance.
- **Betting System Fixes**: Resolved a bug in the betting system related to splitting the first hand of a hand that had already been split.
- **Modular Game Type Objects**: Prepared for the addition of new games by creating new files and making objects more modular.
- **Username Change Exception Handling**: Fixed a bug in the server-side exception raising for changing usernames.
- **Dealer Draw Logic**: Implemented logic to prevent the dealer from drawing more cards if all players bust or have blackjack.
- **Dynamic UI Elements**: Added dynamic positioning for balance text, deal, and leave buttons in the Blackjack game screen to support various screen sizes.
- **Chip/Bet Display Bug**: Fixed an issue where the chip/bet would not display while waiting for other players to ready up.
- **Turn Display Bug**: Corrected the "Your Turn" display bug which previously always indicated it was your turn if you had cards. Now, it only displays during your actual turn.
- **Hand Value Bug Fix**: Fixed a major bug in the hand value calculation function. It now correctly handles aces, adjusting their value to 1 only when necessary and preserving their higher value when it doesn't cause the hand to bust.
- **Blackjack Payouts**: Adjusted Blackjack payouts to the correct 3 to 2 ratio as in casinos.

#### Lobby System Improvements
- **Lobby ID Overhaul**: Lobby IDs are now 4-character random strings, making them more secure and harder to brute force. This required a complete revamp of the lobby ID system.
- **Private Lobby Fixes**: Resolved bugs in the private lobby system which previously prevented joining private lobbies.

#### UI and Modular Code Improvements
- **Separate File for Screen Elements**: Created a separate file to hold all screen elements (buttons, textboxes, etc.), increasing modularity and readability.
- **Textbox Cursor Addition**: Added a cursor to text boxes for better text input navigation.
- **Screen Element Transition**: Implemented a feature allowing screen elements like text boxes and buttons to transition between each other. This allows smoother page navigation using the Enter key.
- **Connection Error Handling**: Improved error handling to display an error page if the servers are down or if the user cannot connect, instead of crashing the app.

#### New Features
- **Blackjack Insurance**: Added the option to take insurance when the dealer is dealt an Ace face-up. This pays 2 to 1 if the dealer has blackjack. Now our Blackjack game offers all aspects of a typical casino Blackjack game.
- **End of Game Display**: Enhanced the end-of-game display to show not only the result but also the amount of money won or lost.
- **Game Icon Change**: Updated the game icon to a chip instead of a snake.

#### Codebase Preparation
- **Modularity Preparation**: Prepped the codebase for adding new casino games.

Make sure to re-download the game above and remove your old version to enjoy these enhancements. As always, if you encounter any issues or have suggestions, feel free to reach out to us.

------------------------------------------------

## Version 1.1 Update

We are excited to announce the release of **Pixel Casino** version 1.1! This update brings a host of new features, improvements, and bug fixes to enhance your gaming experience. Below is a detailed overview of what's new in this version:

### What's New in Version 1.1

#### Revamped Player Betting System
- **Enhanced Bet Storage:** Player bets system was revamped, allowing for improved handling of split hands and enabling the ability to double after splitting. This also allowed us to display your extra bets on the table.

#### Improved Lobby Displays 
- **Visual Updates:** Players can now see the bets of others, as well as indicators showing who is ready and whose turn it is during the game. We've also added other player's hand totals to your screen so no more doing math to determine your friend's hand value.
- **Dealer Speed Adjustment:** The speed of the dealer's actions has been slowed down for a more enjoyable pace. This should now allow all players to see the cards being drawn.

#### New Features
- **Balance Reset:** A feature to reset the user’s balance has been added, no more fear of going broke. This will serve as a placeholder until a fund-adding system is implemented. 
- **Blackjack Payout Adjustment:** Blackjacks after a split no longer pay 2 to 1, aligning with standard casino rules.

#### User Interface Improvements
- **Dynamic UI Elements:** All button and textbox objects now dynamically orient themselves. Their positions are updated whenever you change the game screen size ensuring a responsive and adaptable interface.

#### Bug Fixes
- **Betting Restrictions:** Major flaws that allowed betting beyond a player's bank have been fixed. Players can no longer double or split without sufficient funds. 
- **Double and Split Restrictions:** You can now double a hand when you have split! A former limitation in the game which our new betting system helped solve. The game now follows typical casino rules.

### How to Update

To update to version 1.1, simply download the latest version of the `PixelCasinoV1-1.zip` file from the release page, extract it to your desired location, and replace the previous version. Make sure the `assets` folder remains in the same directory as the game executable.

We hope you enjoy the new features and improvements in **Pixel Casino** version 1.1. Your feedback is invaluable to us, so please don't hesitate to share your thoughts and suggestions!

Happy gaming!

**Pixel Casino Team**

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
