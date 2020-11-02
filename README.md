## BlackJack Game
This game has been developed using Python 3. Enjoy playing!

#### Requirements: 
- Running the program
  - Run using the command in Python 3 interpreter: **python3 blackjack.py**
  - No dependencies

- Assumptions/Choices made
  - Running the program once means player can play only once. If player wants to play again, the program must be ran again
  - Since we don't concern ourselves with card suit, I'm using all 13 cards and multiplying it by 4 to get 52 cards
  
- Design choices made
  - Used functional programming by creating functions and handling each scenario as the game progresses for a user
  - Used list to store card values
  - Used list to add cards for player and dealer

- **Test scenarios**
  - Wrong input: Prompt user to enter required key
  - Initial cards: Displays 2 player cards and calculates total. Hides 1 dealer card, display 1 and hide total
  - Total calculation is accurate
  - BlackJack at initial deal: Player has K A
  - Player stands initially:  Dealer hits scenario
  - Player keeps hitting by entering H until entering S: Player has 2 3 (any cards with total < 21)
    - Player busts: Player crosses 21
    - BlackJack: Player gets 21
    - Player stands under 21: Dealer hits scenarrio
    - Player getting cards with Ace: Score recalculation if above 21
  - Dealer hits: 
    - BlackJack: Dealer gets 21
    - Dealer keeps hitting until 17, crosses 21: Dealer bust
    - Dealer keeps hitting until 17, under 21: Score comparision. Higher scorer wins
    - Dealer keeps hitting until 17, under 21: Score comparision. Tie
  - Display final cards if not blackjack/bust
