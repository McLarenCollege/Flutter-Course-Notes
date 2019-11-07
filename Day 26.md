# Day 26 - Assignments for the day

1. Morning Challenge
2. Refactor [Ashish's code](https://github.com/AshishTaduce/day_25_morning_challenge)
3. Refactor your own Sudoku Code
4. Timezone picker

    **Stage 1**:
    Create a screen which displays timezone property similar to:
 
 ![](screenshots/timezonePicker.jpeg)
 But we want to merge the region and timezone property
     so it should be: Asia/Kolkata (GMT+5.30)
     
 When this item is clicked it should take me to list of all available timezones
 
 ![](screenshots/timezoneList.jpeg)

**Stage 2**: Implement search on list page just like flutter sample app
     
![](screenshots/timezoneList%20Search.jpeg)

5. **Stretch** Add Search functionality to maps app

Load the cities from this [json file](https://github.com/lutangar/cities.json/blob/master/cities.json)

Get rid of the list of cities on page
Have a search button which navigates to search page, show the list of 
cities as and when user types
Have a read of this article to [handle json data](https://flutter.dev/docs/cookbook/networking/background-parsing#4-move-this-work-to-a-separate-isolate)