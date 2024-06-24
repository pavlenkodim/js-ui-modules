# JavaScript Timer Module

This is a simple JavaScript module that provides a countdown `timer` functionality. The timer module allows you to easily create and display a countdown timer on your webpage.

## Usage

To use this timer module, follow these steps:

1. Include the `timer` module in your project.

```
import timer from 'path-to-timer-module/timer.js';
```

2. Create an HTML element where you want to display the timer. Give it an `id` attribute.

```
<div id="myTimer">
    <span id="days">00</span> days
    <span id="hours">00</span> hours
    <span id="minutes">00</span> minutes
    <span id="seconds">00</span> seconds
</div>
```

3. Call the `timer` function, passing the `id` of the HTML element and the deadline for the timer.

```
const deadline = new Date('January 1, 2025 00:00:00');
timer('myTimer', deadline);
```

Replace `'myTimer'` with the `id` of your HTML element and set the `deadline` to the desired date and time for the timer to count down to.

## Functions
### `getTimeRemaining(endtime)`

Calculates the time remaining until the specified `endtime`. Returns an object with properties:

* `total`: Total milliseconds remaining.
* `days`: Number of days remaining.
* `hours`: Number of hours remaining.
* `minutes`: Number of minutes remaining.
* `seconds`: Number of seconds remaining.

### `getZero(num)`

Adds a leading zero to a number if it is less than 10. Used for formatting the timer output.

### `setClock(selector, endtime)`

Sets up the timer display using the provided selector (HTML element id) and endtime.

### `updateClock()`

Updates the displayed timer values and clears the interval if the countdown has reached zero.

## Example

```
import timer from 'path-to-timer-module/timer.js';

const deadline = new Date('January 1, 2025 00:00:00');
timer('myTimer', deadline);
```

Feel free to customize the HTML structure and styling according to your project requirements.