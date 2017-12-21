## The Guess My Number Kata

Let's play a game. I'm thinking of a number, you have to guess it.

## The Kata

Write a method to tell the user whether a whole number between 1 and 100 is greater than, less than, or equal to the number the computer is thinking of.
We can initialize this number using any random number generator.

An appropriate congratulatory message is in order if the user guesses the correct number.

## A First Extension

Initialize the number to guess within an arbitrary range. For the sake of simplicity, negative numbers should be banned.

## Extending further

Instead of saying whether the guess is greater than or less than the stored number, say `warmer` if the absolute difference is less than the previous guess, and `colder` if the absolute difference is greater than the previous guess.

The initial response after the first guess should be cold, warm, or hot depending on how close the user is to the correct number. Come up with reasonable defaults, a suggestion would be to use 10% of the range (rounded to the nearest whole number) for hot, 25% for warm and cold otherwise. Switch to the warmer/colder strategy as of the second guess until the user selects the correct number.