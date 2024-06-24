# JavaScript Forms Module

This JavaScript module facilitates easy handling of forms on your webpage. It includes features for submitting form data asynchronously, displaying loading spinners, and showing a modal with success or failure messages. The module utilizes other modules for modal operations and sending data.

## Installation

Make sure you have the necessary dependencies installed:

```
npm install # or yarn install
```

## Usage

1. Import the module and required dependencies in your JavaScript file:

```
import forms from 'path-to-forms-module/forms';
import { clouseModal, openModal } from 'path-to-modal-module/modal';
import { postData } from 'path-to-services-module/services';
```

2. Call the `forms` function with the appropriate parameters:

```
forms('.your-form-selector', modalTimerId);
```

Replace `.your-form-selector` with the selector for your form and provide the `modalTimerId` for controlling the modal timer.
## Functions

### `bindPostData(form)`

Binds the form submission event to handle the data asynchronously. It displays a loading spinner during the submission process and handles success or failure accordingly.

### `showThanksModal(message)`

Displays a modal with a success or failure message. It hides the original modal content temporarily and appends a new content block with the provided message. After a brief period, it removes the new content and restores the original modal.

## Example

```
import forms from './path-to-forms-module/forms';
import { clouseModal, openModal } from './path-to-modal-module/modal';
import { postData } from './path-to-services-module/services';

forms('.your-form-selector', 5000);
```

Replace the placeholder paths and parameters with your actual paths and values.

Feel free to customize the module's behavior, styling, and error messages according to your project requirements.
