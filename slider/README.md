# JavaScript Slider Module

This JavaScript module provides a flexible and customizable slider functionality for your webpage. You can easily create a slider with next and previous navigation buttons, slide indicators, and automatic sliding.

## Usage

To use the slider module, follow these steps:

1. Include the `slider` module in your project.

```
import slider from 'path-to-slider-module/slider.js';
```
2. Create an HTML structure for your slider with appropriate IDs and classes.

```
<div class="slider-container">
    <div class="slider-wrapper">
        <div class="slider-field">
            <!-- Your slides go here -->
        </div>
    </div>
    <button class="prev-arrow">&lt;</button>
    <button class="next-arrow">&gt;</button>
    <div class="total-counter"></div>
    <div class="current-counter"></div>
</div>
```

3. Call the `slider` function, passing an object with the necessary options.

```
slider({
    container: '.slider-container',
    slide: '.your-slide-class',
    nextArrow: '.next-arrow',
    prevArrow: '.prev-arrow',
    totalCounter: '.total-counter',
    currentCounter: '.current-counter',
    wrapper: '.slider-wrapper',
    field: '.slider-field'
});
```

Replace the class names with your specific class names or IDs.

## Options

* `container`: The selector for the slider container.
* `slide`: The selector for each slide element.
* `nextArrow`: The selector for the next arrow button.
* `prevArrow`: The selector for the previous arrow button.
* `totalCounter`: The selector for the total counter element.
* `currentCounter`: The selector for the current counter element.
* `wrapper`: The selector for the slides wrapper element.
* `field`: The selector for the slides field element.

## Functions

* `switchSlides(next = true)`: Switches to the next or previous slide based on the next parameter.
* `slideCurrent()`: Updates the displayed current slide number.
* `dotsView()`: Updates the visibility of the slide indicators (dots).
* `deleteNotDigits(str)`: Utility function to remove non-digit characters from a string.

## Example

```
import slider from 'path-to-slider-module/slider.js';

slider({
    container: '.slider-container',
    slide: '.slide',
    nextArrow: '.next-arrow',
    prevArrow: '.prev-arrow',
    totalCounter: '.total-counter',
    currentCounter: '.current-counter',
    wrapper: '.slider-wrapper',
    field: '.slider-field'
});
```

Feel free to customize the HTML structure, styling, and options according to your project requirements.