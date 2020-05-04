## Review

You are required to submit the following for review:

- The URL of the deployed application: https://sbonias.github.io/work-day-scheduler/

- The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

## Pseudocode

```
-------------------------HTML Layout.........................
// Requires Timeblocks (referenced the styles.css file for naming conventions and expected elements) x
//      -Each block of time consists of the following components: x
//          -"time-block" = Displays the hour x
//              -this is a static field as the time-blocks start at 9am and end at 5pm (each hr has time-block) x
//          -"textarea" = Allows for user input x
//          -"saveBtn" = Allows for user to save input (local storage) x
//              -embedded padlock icon x
//      -Appears as though I will need a new row per each block (9 blocks in total) x
//      -Appears as though the different sections of the block will be separated into columns x
//          -targeting 3 columns per block x

-------------------------JS Functionality .........................
// Display the Current Date in the corresponding HTML Div x
//      -Format = "Thursday, September 5th" x
//      -Apply moment.js functionality/formatting x
//      -Target currentdate div in HTML doc x
//      -Use jQuery to output value to HTML x
// Will need to create function that updates the background color of the text areas element per the current time x
//      Criteria: x
//      -When the time-block hour = current hour x
//          -text area displays as red x
//      -When the time-block > current hour x
//          -text area displays as green x
//      -When the time-block < current hour x
//          -text area displays as grey x
//      How to accomplish this? x
//          -see "textAreaBackgroundColor" function comments to see how this was accomplished x
// Will need to implement local storage function to text-area div
//      -this will save all tasks entered in the text-area div under the given time block so when refreshing the page your tasks are not emptied
//      -works or saves when save button is clicked (on click event)
// Will need to implement moment.js x
//      -for data and time conversions throughout application x
//          -noticed that this was already linked in the html document x
```

## System Requirements

```
// Requires Moment.js library to work with data and time
//      -https://momentjs.com/
```

## Sources

```
// Using moment.js:
//  -https://www.webfx.com/blog/web-design/javascript-dates-moment-js/
// Creating a text input field in HTML
//  -https://www.w3schools.com/tags/tag_textarea.asp
// Parse Integer:
//  -https://www.w3schools.com/jsref/jsref_parseint.asp
// Calling the ID of an element via jQuery:
//  -https://stackoverflow.com/questions/3239598/how-can-i-get-the-id-of-an-element-using-jquery
// Returning unique id's from multiple similarly named classes
//  -https://stackoverflow.com/questions/33147262/get-id-value-from-multiple-class

```

```
-------------------------Original ReadMe.........................
```

# 05 Third-Party APIs: Work Day Scheduler

Create a simple calendar application that allows the user to save events for each hour of the day. This app will run in the browser and feature dynamically updated HTML and CSS powered by jQuery.

You'll need to use the [Moment.js](https://momentjs.com/) library to work with date and time. Be sure to read the documentation carefully and concentrate on using Moment.js in the browser.

## User Story

```
AS AN employee with a busy schedule
I WANT to add important events to a daily planner
SO THAT I can manage my time effectively
```

## Acceptance Criteria

```
GIVEN I am using a daily planner to create a schedule
WHEN I open the planner
THEN the current day is displayed at the top of the calendar
WHEN I scroll down
THEN I am presented with timeblocks for standard business hours
WHEN I view the timeblocks for that day
THEN each timeblock is color coded to indicate whether it is in the past, present, or future
WHEN I click into a timeblock
THEN I can enter an event
WHEN I click the save button for that timeblock
THEN the text for that event is saved in local storage
WHEN I refresh the page
THEN the saved events persist
```

The following animation demonstrates the application functionality:

![day planner demo](./Assets/05-third-party-apis-homework-demo.gif)

## Review

You are required to submit the following for review:

- The URL of the deployed application.

- The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

---

© 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
