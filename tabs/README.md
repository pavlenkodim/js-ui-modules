# JavaScript Tabs Module

This JavaScript module provides a simple and flexible solution for creating tabbed content on your webpage. The module allows you to define tabs, associated content, and their parent container, making it easy to implement tab functionality.

## Usage

1. Include the `tabs` module in your project.

```
import tabs from 'path-to-tabs-module/tabs';
```

2. Set up your HTML structure with tabs and associated content:

```
<div class="tabs-container">
    <div class="tab" data-tab="1">Tab 1</div>
    <div class="tab" data-tab="2">Tab 2</div>
    <div class="tab" data-tab="3">Tab 3</div>

    <div class="tab-content" data-tab="1">
        <!-- Content for Tab 1 -->
    </div>
    <div class="tab-content" data-tab="2">
        <!-- Content for Tab 2 -->
    </div>
    <div class="tab-content" data-tab="3">
        <!-- Content for Tab 3 -->
    </div>
</div>
```

3. Call the `tabs` function, passing the necessary parameters.

```
tabs('.tab', '.tab-content', '.tabs-container', 'tabheader__item_active');
```

Replace the class names and selectors with your specific values.

## Parameters

* `tabsSelector`: Selector for the tabs.
* `tabsContentSelector`: Selector for the associated content.
* `tabsParentSelector`: Selector for the parent container of tabs.
* `activeClass`: Class to indicate the active tab.

## Functions

### `hideTabContent()`

Hides all tab content and removes the active class from tabs.

### `showTabContent(i = 0)`

Shows the tab content for the specified index (i). By default, it shows the content for the first tab.

## Example

```
import tabs from 'path-to-tabs-module/tabs';

tabs('.tab', '.tab-content', '.tabs-container', 'tabheader__item_active');
```

Feel free to customize the HTML structure, styling, and options according to your project requirements.