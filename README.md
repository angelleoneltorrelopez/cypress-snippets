# VS Code Cypress Snippets
Is a collection of small snippets of predefined code that covers different features and use cases common in UI tests coded with Cypress.

[![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/license/mit/)
![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/angelleoneltorrelopez.cypress-snippets-v2?label=Installs)

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
       cy.visit('url');
   })
   it('test case description', () => {
       // code here
   })
})
```

### Request Get: `cyRequestGet`
```javascript
cy.request('url')
  .then((response) => {
   expect(response.status).to.have.eq(200);
   // assertion code here
});
```

### Request Post: `cyRequestPost`
```javascript
cy.request({
    method: 'POST',
    url: 'url',
    body: {
      parameters: 'value'
    },
  }).then((response) => {
    expect(response.body).to.have.property('parameters', 'value');
  });
```

### Request Put: `cyRequestPut`
```javascript
cy.request({
    method: 'PUT',
    url: 'url',
    body: {
      parameters: 'value'
    },
  }).then((response) => {
    expect(response.body).to.have.property('parameters', 'value');
  });
```

### Request Delete: `cyRequestDelete`
```javascript
cy.request({
    method: 'DELETE',
    url: 'url',
  }).then((response) => {
    expect(response.status).to.eq(204);
  });
```

### Intercept: `cyIntercept`
```javascript
cy.intercept(
    'method',
    'url'
   ).as('name');
```

### Intercept Fixture: `cyInterceptFixture`
```javascript
cy.intercept(
    'method',
    'url',
    {
      fixture: 'example.json',
    },
   ).as('name');
```

### Intercept Status Code: `cyInterceptStatusCode`
```javascript
cy.intercept(
    'method',
    'url',
    {
      statusCode: 500,
    },
   ).as('name');
```

### Command Add: `cyCommandAdd`
```javascript
Cypress.Commands.add('Name', (Parameters) => {
   // code here
  });
```

### Describe: `cyDescribe`
```javascript
describe('test description', () => {
   // code here
})
```

### Context: `cyContext`
```javascript
context('Context', () => {
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

### It: `cyIt`
```javascript
it('Test description', () => {
   // code here
});
```

### After: `cyAfter`
```javascript
after(() => {
   // code here
});
```

### AfterEach: `cyAfterEach`
```javascript
afterEach(() => {
   // code here
});
```

### Visit: `cyVisit`
```javascript
cy.visit('url');
```

### Get: `cyGet`
```javascript
cy.get('selector')
```

### Check: `cyCheck`
```javascript
.check()
```

### Uncheck: `cyUncheck`
```javascript
.uncheck()
```

### Contains: `cyContains`
```javascript
.contains('content')
```

### Find: `cyFind`
```javascript
.find('selector')
```

### Type: `cyType`
```javascript
.type('text')
```

### Clear: `cyClear`
```javascript
.clear()
```

### Click: `cyClick`
```javascript
.click()
```

### Click: `cyDblClick`
```javascript
.dblclick()
```

### Click: `cyRightClick`
```javascript
.rightclick()
```

### Wait: `cyWait`
```javascript
cy.wait('');
```

### Wait Element: `cyWaitElement`
```javascript
.wait('')
```

### Each: `cyEach`
```javascript
.each((el, index, list) => {
   // code here
});
```

### Log: `cyLog`
```javascript
cy.log();
```

### Pause: `cyPause`
```javascript
cy.pause();
```

### Screenshot: `cyScreenshot`
```javascript
cy.screenshot('');
```

### Debug: `cyDebug`
```javascript
cy.debug();
```

### Viewport: `cyViewport`
```javascript
cy.viewport(width, height);
```

### Go Back: `cyGoBack`
```javascript
cy.go('back');
```

### Go Forward: `cyGoForward`
```javascript
cy.go('forward');
```

### Select: `cySelect`
```javascript
.select('')
```

### Select File: `cySelectFile`
```javascript
.selectFile('')
```

### Clear All Cookies: `cyClearAllCookies`
```javascript
cy.clearAllCookies();
```

### Clear All LocalStorage: `cyClearAllLocalStorage`
```javascript
cy.clearAllLocalStorage();
```

### Clear All SessionStorage: `cyClearAllSessionStorage`
```javascript
cy.clearAllSessionStorage();
```

### Force: `cyForce`
```javascript
{ force: true }
```

## License

[MIT](./LICENSE)
