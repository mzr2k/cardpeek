## Card Peek Mechanism - Unity Implementation

This Unity library provides a script for creating a realistic card-flipping effect in your game. The effect simulates the physics of a turning page and includes a configurable shadow effect.

### Features

* Customizable page turning animation
* Supports both left-to-right and right-to-left flipping
* Optional shadow effect for added depth
* Event triggered on page flip

### Installation

1. Clone or download this repository.
2. Add the `Book.cs` script to your Unity project.
3. Attach the `Book` script to a GameObject that represents your book.

### Usage

The `Book` script exposes several properties and methods for controlling the card-flipping effect:

* **canvas:** (Required) A reference to the canvas that the book is a child of.
* **BookPanel:** (Required) A reference to the RectTransform of the gameobject that visually represents the book.
* **background:** (Optional) The sprite to display behind the pages.
* **bookPages:** (Required) An array of Sprites representing the pages of the book.
* **interactable:** (Optional) A boolean value indicating whether the card flipping can be interacted with by the user (defaults to true).
* **enableShadowEffect:** (Optional) A boolean value indicating whether to enable the shadow effect (defaults to true).
* **OnFlip:** (Optional) A UnityEvent that is triggered when the card flipping animation is complete.

**Flipping the Page**

You can initiate the card-flipping animation by calling one of the following methods:

* `DragRightPageToPoint(Vector3 point)`: This method initiates a right-to-left page flip animation to the specified point on the screen.
* `DragLeftPageToPoint(Vector3 point)`: This method initiates a left-to-right page flip animation to the specified point on the screen.

These methods can be called in response to user input events, such as a mouse click or drag.

### Additional Notes

* This script relies on the `ExecuteInEditMode` directive, which allows you to see the card-flipping animation in the Unity editor.
* The archived version of the original blog post referenced in the script can be found [here](https://dandarawy.com/html5-canvas-pageflip/).

### Contributing

Contributions are welcome! Yippee!
