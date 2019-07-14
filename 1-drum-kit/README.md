## Lesson Learned

- To get key code use `charCodeAt` because `keyCode` and `which` API is deprecated.
  ref: https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/keyCode

- We can listen to `transitonend` event for class name that has `transition` property.

- Sometimes `transitionend` event does not work properly and make class name stuck. To solve this, we can add `keyup` event listener to document,
  to make sure no class name is stuck because of `transitionend` listener is not triggered.
