## Create a calendar for a next (2019) year, using React and Bootstrap/Material/Semantic UI for your choise

![Calendar](https://raw.githubusercontent.com/kl2karpenko/MateAcademy/master/React/calendar/cal.png)

## Task
### Base Level

1. The UI of calendar should look based on the picture, means that view should be strengthen on all page and it should have a minimum height so it looks good and don't break
2. Every cell is a day in a month. You should have a nme of Month and year on the top of the page, and arrows `Back` and `Towards` to change the view and render new month. 
3. If you month have less days than cells, don't show cells from other month just leave  them empty


### Middle Level

1. Create an ability to add an event to the calendar on click on the day (on click on a cell)
2. While adding an event you should have a Popup That gives you 3 fields: `date` `name` and `description` of an event
3. After user click `Add` you add an event to this day and hide the Popup


### Advanced Level

1. When User clicks on the special place on the day cell, you can propose the time for an event based on the mouse position in the cell (means if he click lower than the middle it can be 10-12 o'clock and etc.)
2. If you have events that conflicts with each other by `date` just place them in the one row(level) in the cell
