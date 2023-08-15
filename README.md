# Drag and Drop Functionality Example

This is a simple example of implementing drag and drop functionality using JavaScript. The code allows you to drag an item and drop it into various boxes.

## Getting Started

To try out this example, follow these steps:

1. Clone or download this repository to your local machine.
2. Open the `index.html` file in a web browser.
3. You'll see an item that you can drag and drop into the boxes.

## How It Works

1. The code selects the `.item` element, which represents the draggable item.
2. When the item is dragged (`dragstart` event), its ID is stored in the `dataTransfer` object and the item is hidden with a `hide` class.
3. The code selects all `.box` elements (drop target boxes) and adds event listeners for various drag and drop events: `dragenter`, `dragover`, `dragleave`, and `drop`.
4. When the dragged item enters a box, the box gets a `drag-over` class added temporarily (visual feedback).
5. The `dragover` event is used to prevent the default behavior of the browser, which is to disallow dropping.
6. When the dragged item leaves a box, the `drag-over` class is removed.
7. When the item is dropped into a box, the `drag-over` class is removed, and the item is appended to the box's content. The `hide` class is removed, making the item visible again.
