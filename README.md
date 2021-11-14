## Slate Test Utils

Helpers to allow you test Slate within a JSDOM environment with Jest and React Testing Library.

Unfortunately this isn't plug and play. If you have any experience with contenteditable you know that nothing is easy, testing especially.

## Installation

TODO

## Issues

- The new automatic JSX runtime with typescript `react-jsx` doesn't play nice with custom hyperscript. You will need to create a typescript file specific for your tests and use `"jsx": "react"`.
- React 17 will work, but at the moment Slate itself is 16.8. We are going to follow their lead.

## Why

- Test your editor with surgical precision
- Guard your app code from Slate core updates
- Faster and easier to write than Cypress or E2E testing libs
- User driven integration tests give higher confidence
- Simulate OS's by user agent to make sure you are using the right key bindings
- Familiar setup if you already have Jest and React Testing Library
