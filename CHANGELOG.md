# v0.2.9

- Explicity declares lodash dependency used by Eventline

# v0.2.8

- Fixes bug where errors in actions could stop Eventline handling all events in the future

# v0.2.7

- Adds sanity check for older RxJS versions to remind developers to check they are using
  the correct version of RxJS when they are having problems
- Fixes circular json error on built in exception handler

# v0.2.6

- Fixes event showing up as `[object Object]` in exception error message

# v0.2.5

- Removes dependencies on external stack tracing libraries

# v0.2.4

- Fixes issues with previous version not being built correctly

# v0.2.3

- The default exception handler now logs the stack trace to help you understand the
  error

# v0.2.2

- Fixes issues with previous version not being built correctly

# v0.2.1

- Handles events that aren't matched by any route as an error

# v0.2.0

- Strings in patterns are now case-insensitive (i.e "Hello" will match "hello" and "HELLO")
- `Router` renamed to `Eventline` to prevent confusion with the concept of a router for API frameworks. This framework is between a router and a eventbus so this reflects that
- We now handle exceptions and log them to the console to prevent server crashes. You can provide your own exception handler by setting your function on the new `exceptionHandler` property for your eventline.
- We now provide an example for eventline
- We now bundle a simple `when` action by default which allows you to optionally switch on and off individual actions for a route based on pattern matching

# v0.1.0

- Initial Release
