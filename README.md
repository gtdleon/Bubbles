Bubbles
=======

**Xcode UIKitDynamics example**

This example app creates bubbles that are free to float about the screen, within the screen bounds. A bubble can be popped by tapping it, and a new bubble can be created with a long press.

**AppDelegate**

- The app delegate - loads the proper ViewController based on the device type (iPhone/iPad)


**MainViewController/MainViewControlleriPad**

- The main view controller for the app - loads a BubbleView that fills the screen and serves as the BubbleView delegate

**BubbleView**

- A subclassed UIView for controlling the bubbles using a UIDynamicAnimator and randomized UIPushBehaviors to move the bubbles around the screen. A UICollisionBehavior keeps the bubbles from leaving the screen. This view handles creation and deletion of bubbles.

**Bubble**

- A subclassed UIView representing a bubble that consists of a foreground image and a background image, the latter of which is colored with the Bubble tint color. Bubble.m also handles the animation of a bubble popping, and plays a popping sound effect.


