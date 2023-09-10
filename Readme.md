# Calendar App
This repository contains a simple calendar application that allows users to select a month and year, and it displays the corresponding dates for that month. Additionally, the user can enter a specific date, and the application will highlight that date in the calendar.

## Usage
* When you open the application, you'll see a dropdown menu to select a month and a dropdown menu to select a year.
* By default, the current month and year are selected.
* The calendar will display the dates for the selected month and year.
* To change the month or year, simply select a different option from the respective dropdown menu.

## Features
* The application dynamically generates and populates the calendar based on the selected month and year.
* The calendar correctly handles leap years, adjusting February accordingly.
* Users can enter a specific date in the input field, and the application will highlight that date in the calendar.

## Hosted Link
https://ameya-shinde.github.io/Calender2/

## Code Overview
The code is written in JavaScript and utilizes HTML and CSS for the user interface. Here's a brief overview of the main components:
* `index.html`: Contains the structure of the webpage, including the dropdowns, calendar, and input field.
* `styles.css`: Provides styling for the calendar and input field.
* `script.js`: Contains the JavaScript code for generating the calendar, handling user input, and highlighting dates.

## JavaScript Details

### `dateOfFirstDay(month, year)`

- Populates the calendar based on the selected month and year.
- It calculates the first day of the month and calls `fillDates` to fill in the dates.

### `fillDates(day, month, year)`

- Fills in the dates for the selected month and year, accounting for the number of days in each month and handling leap years.

### `highlightColor(date)`

- Highlights the selected date in the calendar.

### `fillingYears()`

- Populates the year dropdown with options ranging from 1950 to 2090.

### `takeinputs()`

- Gets the selected month and year values from the dropdowns and calls `dateOfFirstDay` with the updated values.

### `ValidateDate(e)`

- Prevents the default form submission behavior.
- Gets the date entered by the user.
- Calls `highlightColor` to highlight that date in the calendar.
