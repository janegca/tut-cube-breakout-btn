# tut-cube-breakout-btn

A breakout button
[tutorial](https://piccalil.li/tutorial/create-a-semantic-break-out-button-to-make-an-entire-element-clickable)
using CUBE methodology. A common pattern that requires an area larger than a
link itself to be clickable.

This is not a standalone component, it works in conjunction with a positioned
parent element. Hover and focus effects are needed on both the parent and button
child and work in conjunction with each other.

- The button's parent element is positioned.
- The button itself retains the default `static` position.
- An overlay is added to the `button` in the `::before` pseudo-element. It's
  position set to is set to `absolute` and it becomes positioned relative to the
  button's nearest positioned ancestor, not the button itself; it is this
  technique which makes the button's parent entirely clickable.
