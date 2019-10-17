# Day 12 - Network Calls and Weather App


# Assignments for the day

1. Morning Challenge [Starter code](https://github.com/McLarenCollege/day_12_morning_challenge)
2. Weather App Part 1
    - Make sure you are fetching Location coordinates
    - Make sure you are making weather request to real Api url
        - Signup on [OpenWeather here](https://home.openweathermap.org/users/sign_up)
        - After sign up [go to this page](https://home.openweathermap.org/api_keys) to get the api key
        - Use the api key in this url to make the request for real data - - `https://api.openweathermap.org/data/2.5/weather?lat=19&lon=72&appid=$API_KEY_HERE`
    - Pass in the latitude and longitude to the url and get local weather data
    - Pass json data from weather screen to location screen and display real temperature 
    
    
3. Kismet App Improvements
    - As of now we are using if/else blocks to navigate the stories. Imagine having longer stories, it would mean more if/else block.
    Basically not a scalable way of creating app.
    - Use the [JSON data](https://gist.githubusercontent.com/McLarenCollege/45f2c0107d9436b2f64a588cbd243a6a/raw/09fb409998a24a5dfdf0f7b378e58284c9e3423e/kismet_story.json) to modify the `story` class 
    - Refactor storyBrain 
    
4. **Stretch** Quotes Application
    - Build Quotes app from Scratch [Starter Repository](https://github.com/McLarenCollege/quotes_app_starter)
    - The starter repo contains bare minimum layout
    - Make a network request to `https://favqs.com/api/qotd`
    - design the layout and display the quotes
    
    - Create quote class (You decide the fields)
    - Use the class to convert json to list of quotes
    
    ![](screenshots/QuotesApp%20UI.png)