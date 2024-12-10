# Uncommon HTML Bug: innerHTML and Dynamic Event Listeners

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML when dynamically adding content that includes event listeners.  The bug arises from how `innerHTML` handles event listeners within dynamically added content, often leading to unexpected behavior.

## The Bug
The bug is demonstrated in `bug.html`.  The code attempts to add a button with an `onclick` event listener using `innerHTML`.  However, this method doesn't correctly attach the event listener, resulting in unexpected behavior or no functionality.

## The Solution
The solution is provided in `bugSolution.html`.  Instead of using `innerHTML`, it uses a more robust approach involving `createElement`, `appendChild`, and explicit event listener attachment to ensure correct functionality.

This approach is safer and prevents the inconsistencies associated with `innerHTML` when handling dynamic content and event listeners.