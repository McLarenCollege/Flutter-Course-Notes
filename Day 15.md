# Day 15 - Refactoring Tic Tac Toe Part 2

Continued from previous day:

5.  Use Token instead of String to represent current player
    - Refactor winnerPopup() into two distinct functions: 
        1. Change player if game is not finished
        2. Get the status text   
    - Write test cases to each new function
6. Use `GestureDetector` instead of FlatButton


## Assignment for the Day!
1. Morning Challenge [Starter Repository](https://github.com/McLarenCollege/day_15_morning_challenge)
2. Refactoring point 5 and 6
3. Fit And finish of new york time clone
    - Make sure you have two screens as shown:

    ![](screenshots/NewYorkScreen%20Layout.png)

    ![](screenshots/NewsDetailPage%200.png)
    ## In first screen
    - In first screen, get the font of heading and description to be of serif family
    - Handle null values lookup `??` operator in dart
    - Spacing is important
    - Description text top align
    - Images of the same size
    - Remove source from the title
    - Handle overflow of the text
    
    ## **In second screen**
    - Add placeholder caption to the image as it is not provided by the API
    - See image is going from left end to right end
    - Time format and author name correct
    - Handle null cases as well
    - Have app bar with action buttons
    - Proper font and styling applied
        
    ![](screenshots/NewsDetailPage%200.png)
    
    ![](screenshots/NewsDetailPage.png)

    
4. Currency Exchange Rate [Starter Repo](https://github.com/McLarenCollege/currency_exchange_app)
   Create an app having layout like this:
   
   ![](screenshots/Currency%20Exchange%20Android.png)
   
   You can use this [Exchange Rate API service](https://exchangeratesapi.io/) to fetch the exchange rates
   
   If this app is opened in iOS you should show iOS specific choice picker as shown here:
   
   ![](https://flutter.dev/images/widget-catalog/cupertino-picker.png)
   
5. **Stretch** New York Times Modification
    - Use hero animation to animate the image from list to detail page
    - Implement pull to refresh on news list page
    - Use image plugin to make the image interactive (zoom in and zoom out in separate screen)