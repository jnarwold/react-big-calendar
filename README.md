# react-big-calendar

WARNING: This is a package exclusively for development until an official release is issued

An events calendar component built for React and made for modern browsers (read: IE10+) and uses flexbox over the classic tables-ception approach.

[**DEMO and Docs**](http://intljusticemission.github.io/react-big-calendar/examples/index.html)

Inspired by [Full Calendar](http://fullcalendar.io/).

## Use and Setup

`npm install react-big-calendar --save`

Include `react-big-calendar/lib/css/react-big-calendar.css` for styles, and make sure your calendar's container
element has a height, or the calendar won't be visible.

## Run examples locally

```
$ git clone git@github.com:intljusticemission/react-big-calendar.git
$ cd react-big-calendar
$ npm install
$ npm run examples
```

* Open [localhost:3000/examples/index.html](http://localhost:3000/examples/index.html).

### Localization and Date Formatting

`react-big-calendar` includes two options for handling the date formatting and culture localization, depending
on your preference of DateTime libraries. You can use either the [Moment.js](http://momentjs.com/) or [Globalize.js](https://github.com/jquery/globalize) localizers.

Regardless of your choice, you **must** choose a localizer to use this library:

#### Moment.js

```js
import BigCalendar from 'jnarwold-react-big-calendar'
import moment from 'moment'

BigCalendar.setLocalizer(BigCalendar.momentLocalizer(moment))
```

#### Globalize.js v0.1.1

```js
import BigCalendar from 'jnarwold-react-big-calendar'
import globalize from 'globalize'

BigCalendar.setLocalizer(BigCalendar.globalizeLocalizer(globalize))
```
