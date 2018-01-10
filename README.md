# Deck-of-Cards

Deck of Cards
Objective
In Swift Structs and Classes are used extensively. This assignment is designed to help you understand the differences between Classes and Structs so that you can choose the best construct for your needs when building your own applications. It is natural to question whether to use a Class or a Struct, and this will become more and more clear as you use both and see the differences.

With this assignment we will be building the basic structure of a simple game we are going to call "Machi". For this game there are 30 cards of 3 different colors each with a value that matches one of the potential rolls of a six-sided dice.

To Do
Create a struct called "Card"

Give the Card struct a property "Color" which will hold the color values associated with the card (Red, Blue, or Green). This value should be a String or an Enum
Give the Card a property "Roll" which will hold a random value that represents the side of the die that will trigger that card.
Blue cards should have a roll value of either 1 or 2
Red cards should have a roll value of either 3 or 4
Green cards should have a roll value between 4 and 6
Next, create a class called "Deck"

Give the Deck class a property called "cards" of type [Card]
When initializing the deck make sure that it has 10 cards of each color for a total of 30
Give the Deck a deal method that selects the "top-most" card, removes it, and returns it
Give the Deck a isEmpty method that returns true or false in regards to if the deck has ran out of cards.
Give the Deck a shuffle method that randomly reorders the deck's cards
Finally, create a class called "Player"

Give the Player class a name property
Give the Player a hand property of type [Card]
Give the Player a draw method of type (Deck) -> Card which draws a card from a deck, adds it to the players hand, and returns it
Note how we are passing the Deck by reference here since it is a class. 
Give the Player a rollDice method that returns a random number between 1 and 6
Give the Player a matchingCards method of (String, Int) -> Int that will count all the card the player has which match the given color string and roll integer.
