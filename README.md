# Blackjack Game

## Overview
This is a simple implementation of the Blackjack card game in Python. It was created for pure practice and learning purposes, and is by no means original.

## Features
- Allows one player to play against the computer dealer.
- Implements standard Blackjack rules, including player decisions (hit, stand) and scoring.
- Provides a basic command-line interface for interaction.

## How to Play
- Decide how many rounds you want to play and enter the number in integer form. 
- To win blackjack, you would want to have a value as close to 21 as possible, however if you exceeds 21 you loses automatically.
- You would only be able to see one of the dealer's card and if you choose to stand and neither you nor the dealer has a blackjack or have a sum of 21 then the person with a greater number wins.
- Have fun:)

## Project Structure
- **Card**: The Card class allows the user to create a card object with a suit and a rank.
- **Deck**: The Deck class allows the user to create a deck object which is a list collection of cards with suits, rank, and values according to the rank. We used a library to match the rank and values accordingly. There are two methods: shuffle and deal.
    - The Shuffle method returns the card collection in different order with the help of the random module.
    - The Deal method takes in an integer and returns the given number of cards from the end of the collection by removing it from the original deck.
- **Hand**: The Hand class allows the user to create the cards each character has in hand along with the functions that does cards can have. It can be the card of the player or the cards of the dealer. The methods includes add_card, calculate_value, get_value, is_blackjack, and display.
    - add_card method adds the card to the person that called the method and returns nothing.
    - calculate_value method calculates the total value of the cards and returns nothing.
    - get_value method returns the value of the cards of the player.
    - is_blackjack method returns true when the player's cards sum up to the value of 21.
    - display method is a more complicated to String method that shows all the cards of the character is the player while hides most of the cards and only show one card if the person is the dealer.
- **Game**: This is the runner for the blackjack game that interact with the user.

## Acknowledgments
- The game was developed as part of Python learning and practice. It is by no means original.
- Thanks to FreeCodeCamp.org @ https://youtu.be/eWRfhZUzrAc?si=F3-IZhp0ZLsKM9Uu for teaching me beginner python and guiding my through the steps of coding blackjack.
- Thanks to WikiHow @ https://www.youtube.com/watch?v=eyoh-Ku9TCI&ab_channel=wikiHow for explaining how blackjack works.

## Future Improvements
- The code would be more readable if there are comments to explain each step.
- I should also test out corner cases to make sure errors are being handled.
