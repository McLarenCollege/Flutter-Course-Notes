# Welcome to Flutter Course
### You will find day wise notes of the course here

## Structure of the notes
- Content on the topics covered
- Link to Classroom exercises
- Assignments for the day

# Day 1 - Layouts in Flutter

## Introduction  
- Daily Schedule
    - Start at 8.30 AM with a 30 min **challenge**
    - 9 AM to 9.15 AM we review the challenge
    - 9.15 AM to 12.00 PM : **Lecture**
    - 12.00 PM to 12.45 PM : **Lunch Break**
    - 12.45 PM to 4.45 PM : **Project Work**
    - 3.00 PM to 4 PM : **One on One Meetings** (For student it will be just a 5-10 min call)
    - 4.45 PM to 5.00 PM: **Check In** the code
- You Must Show Commitment to the Course
    - We will check your attendance each day.  If you fail to attend a day 
    we will generally give you access to the video and you can catch up, but this 
    counts as a 'strike'.  (We may make an exception if you have an emergency 
    and contact us *before the class starts*).
    - You must submit class exercises when they are due each day.  If you fail
    to submit any of the exercises then (a) you will have to complete the exercise
    within 24 hours; and (b) you will be assigned extra weekend work to catch up.  If you 
    fail to submit the exercise within 24 hours from the deadline time 
    then it will count as a strike.  If you fail to do the weekend catchup work by midnight on Sunday then it will 
    count as a strike.  
    - If you accumulate 3 strikes then we will drop you from the course
    
- Communication Skills Are Extremely Important
    - Webcam should be on all the time
    - Facing camera, Good lighting, good audio and no background noise (if you have background noise please mute it) 
    - With clients: presentation matters, formal attire, clean background in video
    - Check for understanding: 'Let me just make sure I understand' -> example, edge case
    - On Zoom it's very important to respond with 'hi' or 'sure' or 'ok' when
    someone calls on you.


## How to fix errors?

 1. Read and try to understand error messages
 2. Compare syntax with sample code known to work
 3. Comment out code until it compiles, then slowly add code until you encounter an error
 4. Google it, then try to understand the stack overflow answer. Read the best answer, read the official documenation for method calls, etc.
 5. Print debugging (or with proper IDE debugger)
 6. Try different way to write the same logic (Ex sorting in reverse order)

## Optional and Named Parameters in Dart
```dart
void main() {
  fullName('Arnav', 'Puri');
  calculateTotalBill(200, tip: 50); // 250
  calculateTotalBill(150); // 150
}
// function with middleName as optional parameter
  void fullName(String firstName, String lastName, [String middleName]) {
      print('$firstName $middleName $lastName');
  }
  // function with tip as optional and named parameter, it also has a default value of 0
  double calculateTotalBill(double billTotal, {double tip = 0}){
    return billTotal + tip;
  }
```

## Running Flutter App

[Starter Code](https://github.com/McLarenCollege/day1_scaffolding)

### Current Widget Tree
![](screenshots/day1_widget_tree_1.png)

**How can we center the Text on Screen?**
We can use a `Center` widget

The code would look like this
```dart
    void main(){
      String msg = 'Hello World';
      Text textWidget = Text(msg);
      Center center = Center(textWidget);
      MaterialApp myApp = MaterialApp(home: center);  
      runApp(myApp);
    }
```
But more common way of writing this is in one line, so the code would look like this:
```dart
    void main() => MaterialApp(home: Center(Text('Hello World'),),);
```

Better formatted with `dartfmt`.

### Scaffolding an App
Scaffolding means a structure. Flutter has a library called `material` which we import in almost all Flutter related code. It provide a nice way to create an app which has an `AppBar` and `Body` and several other features

Whenever you start learning something new, always remember to checkout documentation of that topic, in this case [Scaffolding](https://api.flutter.dev/flutter/material/Scaffold-class.html)  it is super helpful.

[Mid Day Repo](https://github.com/McLarenCollege/day1_mid_start)

Scaffold consist of two major components, appBar and body,

![](screenshots/scaffold_diagram.png)


### Exercises for the day:
 1. Create a layout to look like this:
 
      ![](screenshots/day_1_assignment.png)
      
[Starter Repository](https://github.com/McLarenCollege/Day-1-Scaffold-assignment)
       
 2. Stretch - Add floating action button with an icon
 
 ![](screenshots/day_1_stretch_assignment.png)
 
 3. [Dart chain Link Exercise](https://github.com/McLarenCollege/dart_chain_link)
 
 4. [Fibonnaci Series](https://github.com/McLarenCollege/fibonnaci_day_1_assignment) 