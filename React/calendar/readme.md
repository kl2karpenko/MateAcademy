## Create a calendar, using React and Bootstrap/Material/Semantic UI for your choise

![Calendar](https://raw.githubusercontent.com/kl2karpenko/MateAcademy/master/React/calendar/cal.png)

### Main stuff:
1. Calendar should start from `2010` year and ends in `2020`
2. If users click to `2020` year `Next` button should be disabled, the same or `2010` and `Previous`

## Task
### Base Level (Full view Calendar)

1. The UI of calendar should look based on the picture, means that view should be strengthen on all page and it should have a minimum height so it looks good and don't break
2. Every cell is a day in a month. You should have a name of Month and year on the top of the page, and arrows `Previous` and `Next` to change the view and render next/previous month. 
3. If you month have less days than cells, don't show cells from other month just leave  them empty


### Middle Level (Single Day View)
![Calendar](https://raw.githubusercontent.com/kl2karpenko/MateAcademy/master/React/calendar/cal-day.png)

1. Create a view to a single day on click on the cell of the day, and `Back` button to return to the whole view Calendar.
2. Add  ability to add an event to the current day when you are on the `Day View` on click on the left side of the day (in the events list)
![Calendar](https://raw.githubusercontent.com/kl2karpenko/MateAcademy/master/React/calendar/cal-day-add-event.png)
2. While adding an event you should have a form on the right side of the page that gives you 3 fields: `date` `name` `description` and `DELETE` button for event.
3. After user click `Add` you add an event to this day and hide form on the right side and add an event to the calendar
4. On click on `DELETE` event button, the event deleted from the calendar
5. On click on existing event, you open the same form on the right with the datail information about the event that was clicked
6. Add icon of weather to the cells, and add functionality to show User what weather will be on that day based on ajax request to https://openweathermap.org/api API when user clicks on `weather icon`. If the weather is unavailable Make a Default Component with some text like: "WE HAVE NO INFORMATION ABOUT WATHER FOR THIS DAY"


### Advanced Level (Additional functionality)

1. If you have events that conflicts with each other by `date` just place them in the one row(level) in the cell
2. If user adds event in the same time, check if time in this day is taken and proppose other time with notification (alert) or some modal
3. Add Drag-And-Drop functionality for the events, to be able to change the vents time table by draggin it in the day cell
4. Add a `REPEAT` select, to add posibility to repeat an event to the other days.
