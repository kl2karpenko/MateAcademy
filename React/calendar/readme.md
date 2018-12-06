## Create a calendar, using React and Bootstrap/Material/Semantic UI for your choise

![Calendar](https://raw.githubusercontent.com/kl2karpenko/MateAcademy/master/React/calendar/cal.png)

### Main stuff:
1. Calendar should start from `2010` year and ends in `2020`
2. If users click to `2020` year `Next` button should be disabled, the same or `2010` and `Previous`

## Task
### Base Level

1. The UI of calendar should look based on the picture, means that view should be strengthen on all page and it should have a minimum height so it looks good and don't break
2. Every cell is a day in a month. You should have a name of Month and year on the top of the page, and arrows `Previous` and `Next` to change the view and render next/previous month. 
3. If you month have less days than cells, don't show cells from other month just leave  them empty


### Middle Level

1. Create an ability to add an event to the calendar on click on the day (on click on a cell)
2. While adding an event you should have a Popup That gives you 3 fields: `date` `name` and `description` of an event
3. After user click `Add` you add an event to this day and hide the Popup
4. Add icon of weather to the cells, and add functionality to show User what weather will be on that day based on ajax request to https://openweathermap.org/api API when user clicks on `weather icon`. If the weather is unavailable Make a Default Component with some text like: "WE HAVE NO INFORMATION ABOUT WATHER FOR THIS DAY"


### Advanced Level

1. When User clicks on the special place on the day cell, you can propose the time for an event based on the mouse position in the cell (means if he click lower than the middle it can be 10-12 o'clock and etc.)
2. If you have events that conflicts with each other by `date` just place them in the one row(level) in the cell
