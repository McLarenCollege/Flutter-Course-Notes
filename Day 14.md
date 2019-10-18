# Day 14 - Refactoring Tic Tac Toe

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

4. Don't duplicate code which creates cells and rows

5.  Use Token instead of String to represent current player
    - Refactor winnerPopup() into two distinct functions: 
        1. Change player if game is not finished
        2. Get the status text   
    - Write test cases to each new function
6. Use `GestureDetector` instead of FlatButton
 
## Assignment for the Day!

### 1. Refactoring from morning
- Do points 1, 2, 3 and 4 from above
    
### 2. New York Times Clone - This is what you have to make

![](screenshots/DemoNewYorkTImes-min.gif)

#### Steps to achieve this
1. Use this [starter repo](https://github.com/McLarenCollege/newyork_times_clone_starter) and make a `NewsCard` Widget, add it to NewsListPage
 - You can add any content you like at this point but get the layout right
 
![](screenshots/news_card.png)
 
2. Repeat the `NewsCard` in a `ListView` to make screen scrollable, you can have different content on these cards to have something like this

![](screenshots/NewYorkScreen%20Layout.png)

3. Fetch Real Data from `https://newsapi.org`, you will have to sign up for free account to get api key
    - Create a network helper to call the api, parse the data into list of newsItem
    - Make sure to handle scenarios when you are not given `urlToImage` parameter 
    
4. Use the fetched data and `ListView.builder` to build list of real news

5. On tap of any news Item open the news detail page (new widget `NewsDetailPage`) which looks like this
    - Make sure it is scrollable
    - the caption of image is a placeholder text as the API doesn't supply that
    
![](screenshots/NewsDetailPage%200.png)

![](screenshots/NewsDetailPage.png)

6. Pass the real data from newsCard to `NewsDetailPage` 