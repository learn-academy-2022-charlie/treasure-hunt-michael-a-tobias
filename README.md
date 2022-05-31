# React Treasure Hunt Game

### Remember:
- Pseudocode!!
- Ask clarifying questions

### User Stories
- As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square. (done)
    - branch: board-game
    - rendered done square with the Square component
    - mapped over square to get nine squares
    - styled group of squares using flexbox
    - passed value of array to Square
    - assigned keys using index
- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array. (done)
    - branch: alert-info
    - pass index to Square component
    - Add an onClick to Square
    - Pass a method from App to Square to get the index
    - centralized the logic so that App.js is the one alerting the index numbers, rather than from the Square component
- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji. (done)
    - branch: tree-emoji
    - destructure board out of state
    - update the board value for the given index
    - use emoji keyboard ctrl + command + space
    - set state with updated value
- As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
- As a user, I can click on a “Play Again” button that will restart the game.
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).