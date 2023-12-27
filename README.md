# Set Game Card Decoder

## Introduction
The Set Game is a challenging and fun card game that tests players' ability to identify patterns and sets from a collection of cards. Each card in the Set Game features four distinct attributes: number, color, shape, and shading. A "set" consists of three cards where each attribute is either all the same on each card or all different.

This Python aims to create a machine learning solution that automates the recognition of cards from the daily SET puzzle and identifies all valid sets within the game. Initially, the project will focus on developing a robust algorithm to decode sets based on the rules of the game. This foundational script serves as a critical component for the larger goal, which involves integrating image recognition and machine learning to process and analyze the daily puzzles automatically.

The idea arose from an informal competition with some friends, where we tried to solve the [online daily set](https://www.setgame.com/set/puzzle) in the fastest time possible.

[The game is hyperlinked if you want to try your luck!](https://www.setgame.com/set/puzzle)

## How the Game Works

In the Set Game, each card has four attributes:

- *Number*: The number of shapes on the card (one, two, or three).
- *Color*: The color of the shapes (e.g., red, green, blue).
- *Shape*: The shape of the symbols (e.g., oval, squiggle, diamond).
- *Shading*: The shading of the shapes (e.g., solid, striped, outlined).

There are 81 different card combinations.

A **set** consists of three cards, where for each attribute, the cards are either all the same or all different. For more information about the game and its rules, check out [Set Game Official Website](https://www.setgame.com/sites/default/files/instructions/SET%20INSTRUCTIONS%20-%20ENGLISH.pdf).

## Project goal
This project aims to develop a machine learning solution capable of recognizing cards from the daily puzzle available at SET Game Online Puzzle and identifying the 6 valid sets required by the game.

An example of what the daily game looks like:
<img width="759" alt="Captura de pantalla 2023-12-27 a las 21 11 59" src="https://github.com/gadeatric/set-game-decoder/assets/115489745/c65c4bb0-5c9a-40a9-8287-58177baa0058">


## Functionality of the Script  
This is a complex project that will be divided into multiple stages. For now, only the logic behind the set decoder has been developed. Other requirements for the completion of the project (data collection, tagging of the cards, training, and development of the model) are still in the works.

The script takes three cards as input, where each card is represented as a list of attributes in the order: number, color, shape, and shading. It then checks whether these three cards form a valid set according to the game rules.

Thi

## How to Use
Each card should be input as a list: ['number', 'color', 'shape', 'shading'].
Call the function with three cards as arguments: is_set_raw(card1, card2, card3).
The function returns a message indicating whether the cards form a set or not.
Example:

```python
card1 = ['1', 'green', 'oval', 'stripped']
card2 = ['2', 'green', 'oval', 'stripped']
card3 = ['3', 'red', 'diamond', 'outlined']
---
is_set(card1, card2, card3)
```
Output
The function returns a string message:

"It's a set!" if the three cards form a set.
"Not a set: ..." with a specific reason if the three cards do not form a set.

## Conclusion

This script is a quick and efficient way to validate sets in the Set Game, enhancing the gaming experience by reducing the time spent on manual validation. Feel free to use and modify this tool to suit your Set Game adventures!
