# VS Code Cypress Snippets
Is a collection of small snippets of predefined code that covers different features and use cases common in UI tests coded with Cypress.

## Installation

To install the snippets in Visual Studio Code, you must first open the command palette (Ctrl + Shift + X or Cmd ⌘ + Shift + X). In the command palette, find "Cypress Snippets" and select it.

## Supported Languages (file extensions)

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)

## Snippets

### Cypress Test Project: `cyProject`
```javascript
describe('This is your test project title', () => {
   beforeEach(() => {
       cy.visit('url')
   })
   it('test case description', () => {
       // code here
   })
})
```

### Describe: `cyDescribe`
```javascript
describe('test description', () => {
   // code here
})
```

### Context: `cyContext`
```javascript
context('', () => {
   // code here
});
```

### Before: `cyBefore`
```javascript
before(() => {
   // code here
});
```

### BeforeEach: `cyBeforeEach`
```javascript
beforeEach(() => {
   // code here
});
```

## License

[MIT](./LICENSE)