# Day 13 - Refactoring Tic Tac Toe

1. Fit and finish
    - Better background
    - Larger icons
    - Stronger highlighted cells
    - Cover fit
    
2. Fix fullBoard

3. Remove Flutter dependencies in gamelogic.dart
    - Use enum instead of x and o widgets
    - Use List<List<Token>> for board
    - Use List<List<Token>> for colorBoard
    - use a method to convert enum or bool to the appropriate widget

4. Use Token instead of String to represent current player
    - Refactor winnerPopup() into two distinct functions: 
        1. Change player if game is not finished
        2. Get the status text   
    - Write test cases to each new function

5. Don't duplicate code which creates cells and rows
 