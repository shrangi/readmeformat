# CalendarJS

This is a JavaScript calendar that is intended to be flexible for entering events or reminders on certain dates.

#### How to use

- Load CalendarJS.js and CalendarJS.css into your project.
- Instantiate the CalendarJS class in your application and enter the div ID that will receive CalendarJS:

```
const calendarJS = new Calendar();
calendarJS.render('#calendar');
```

- You can insert events using the **addEvents** method like this:

```
calendarJS.addEvents(
    [
         {
            name    : 'DocePipoca',
            data    : '17-3-2019',
            hora    : '22:00',
            autor   : 'Mario',
            link    : 'link to the event',
        },
         {
            name    : 'Event name',
            data    : '10-10-2018',
            hora    : '07:00',
            autor   : 'Jeconias',
            link    : 'link to the event',
        }
    ]);

```

- You can render the calendar before or after entering events:

```
const calendarJS = new Calendar();
calendarJS.render('#calendar').addEvents(arrayObj);

// or

calendarJS.addEvents(arrayObj).render('#calendar');
```

#### Available Methods

| Method    | Parameter    | Action                       | Return                 |
| --------- | ------------ | ---------------------------- | ---------------------- |
| render    | ID           | Render calender              | Returns public methods |
| addEvents | Object array | Inserts events into calender | --                     |

#### Changelog

- v0.1 - initiated ;)

#### Current calender style:

![Current Calendar Style](./images/calendarJS.png)

When you click on some event date:

![Current calendar style](./images/specific_date.png)
