Functions of the deck/blackjack:
  1. Drawing a single card randomly (popping top card) <- may revist 
  2. Showing each card (Printing) <- implemented
  3. Comparing card values (comparing hand values) <- value() exists on Card, no logic made yet
  4. Shuffling a deck <- implemented
  5. Duplication checks <- not yet implemented
  6. Deck size checks <- not yet implemented
  7. Initializing deck (Shuffle first) <- Not yet implemented auto-shuffle
  8. Resetting a deck <- Not yet implemented
  9. Hand value logic (Aces) <- not yet implemented
  10. Check for bust (Greater than 21) <- not yet implemented
  11. Check for blackjack (natural 21) <- not yet implemented
  12. Deal initial hands <- not yet implemented
  13. Hit <- not yet implemented
  14. Stand <- not yet implemented
  15. Dealer Logic <- not yet implemented
  16. Win/Loss Logic <- not yet implemented

Test Logic:
  1a. Check if drawn card is a valid Card object (not null)
  1b. Check no card drawn twice without reshuffling
  2a. Check displayCard() returns correct format
  3a. Check face cards (J, Q, K) return 10
  3b. Check number cards return their face value
  3c. Check Ace returns 11 by default
  4a. Store deck order before shuffle, assert check order is different after
  4b. Confirm deck still has 52 cards after shuffle 
  5a. Draw all 52 cards, confirm no duplicates blocked
  6a. Assert new deck has exactly 52 cards
  6b. Assert deck size decrease by 1 after draw
  7a. Assert deck has 52 cards on initialization
  8a. Call reset() and assert deck returns to 52 cards
  9a. Hand with Ace + 10 = 21
  9b. Hand with Ace + 5 + 8 = 14 (Ace has to drop to 1)
  10a. Hand value > 21 returns true for isBust()
  10b. Hand value <= 21 returns false for isBust()
  11a. Two card hand worth 21 returns true for isBlackJack()
  11b. Three card hand worth 21 returns false for isBlackJack()
  12a. After dealing check player has 2 cards, dealer has 2 cards and deck has 48
  13a. After hit, player hand size increases by 1
  14a. Stand returns without adding a card
  15a. Dealer draws until hand >= 17 then stops
  16a. Player 21 vs Dealer 18 : Player wins
  16b. Player 18 vs Dealer 21 : Dealer wins
  16c. Player 20 vs Dealer 20 : Tie
  16d. Player bust : Dealer wins
  
  
  

# Write test logic code here:
