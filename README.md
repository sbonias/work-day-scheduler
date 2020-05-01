## Pseudocode

```
-------------------------HTML Layout.........................
// Require Timeblocks (referenced the styles.css file for naming conventions and expected elements)
//      -Each block of time consists of the following components:
//          -"time-block" = Displays the hour
//              -this is a static field as the time-blocks start at 9am and end at 5pm (each hour has a time-block)
//          -"textarea" = Allows for user input
//          -"saveBtn" = Allows for user to save input (local storage)
//              -represented as a padlock icon
//      -Appears as though I will need a new row per each block (9 blocks in total)
//      -Appears as though the different sections of the block will be separated into columns
//          -targeting 3 columns per block

-------------------------JS Functionality .........................
// Display the Current Date in the corresponding HTML Div
//      -Format = "Thursday, September 5th"
//      -Apply moment.js functionality/formatting
//      -Target currentdate div in HTML doc
//      -Use jQuery to output value to HTML
// Will need to implement local storage function
//      -this will save all tasks to the time blocks
// Will need to implement moment.js
//      -for data and time conversions throughout application
//          -noticed that this was already linked in the html document
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

* The URL of the deployed application.

* The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

- - -
© 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
