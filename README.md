# Blackjack

1. Set all 52 cards following with the given variables(suits, ranks, and values) and playing = True(for continue looping the game)

2. Card class - Set the card and return the detail of each card

3. Deck class - Create the blackjack deck card with all 52 cards by calling the Card-class

	- It can show, shuffle and remove card from deck
  
4. Hand class - This class calculates the value of on-hand card

	- Add card to on-hand and keep track the amount of Ace card
  
	- Adjust Ace value when all cards value over than 21, reduce Ace card value from 11 to 10
  
5. Chips class - This class updates the on-hands player's chips

	- Set default value of chips to 100
  
	- When the player wins, increase the total chips
  
	- When the player loses, reduce the total chips
  
6. Take_bet function - Get the input amount of chips that the player would like to bet in each round.

	- Check if the input is an integer value with try/except 
  
	- Check the amount of the bet if it is not over than the on-hands player's chips
  
7. Hit function - It can be called when the player decide to hit or the dealer's on-hand card value is less than 17

	- Take one card from deck and add it to the on-hand cards
  
8. Hit_or_Stand function 

	- Asking player to decide either Hit or Stand
  
	- If Hit, take more card from a deck
  
	- If Stand, move to the dealer's turn
  
9. Show card function

	- Show_some, this function uses to show all of the on-hand cards with one hidden dealer's card
  
	- Show_all, this function uses to show all of the on-hand cards when the game is over
  
10. 5 Game scenarios (player's view)

	- If the player's value > 21, the player loses
  
	- If the dealer's value > 21, the player wins
  
	- If the player's value > the dealer value, the player wins
  
	- If the player's value < the dealer value, the player loses
  
	- Else, the player ties with the dealer
  
11. Finally, let's start the game.

	- Create a deck card and then shuffle 
  
	- Set the dealer card, the player card and the player chips
  
	- Ask for the amount of the player's bet
  
	- Show the cards with show_some function which the dealer will still hold one hidden card
  
	- It always starts with the player's turn, ask for Hit or Stand
  
	- If choose Hit, it will show the cards with show_some function again
  
	- It's still looping to ask the player until the value of the on-hand player cards exceed 21 or the player decides to stand
  
	- If the value of the on-hand player cards exceed 21, return the outcome scenario as the player busts
  
	- If the player decides to stand and does not bust, it's the dealer's turn with hit function
  
	- Show the cards with show_all function, declare all cards on both sides
  
	- Decide the outcome with other 4 scenarios
  
	- Calucate the final player's chips after the outcome 
  
	- Ask if the player want to play the game again or not
  
