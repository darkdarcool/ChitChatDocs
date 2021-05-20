---
sidebar_position: 1
---

# Tutorial Intro

export const Highlight = ({children, color}) => (
  <span
    style={{
      backgroundColor: color,
      borderRadius: '2px',
      color: '#fff',
      padding: '0.2rem',
    }}>
    {children}
  </span>
);

export const Linkto = ({children}) => (
  <span
        style={{
          textDecoration: 'none',
          color: '#add8e6',
        }}>
        {children}
  </span>
);
<Highlight color="#25c2a0">Docusaurus green</Highlight> and <Highlight color="#1877F2">Facebook blue</Highlight> are my favorite colors.

Let's discover **ChitChatjs in less than 5 minutes**.

## Getting Started

Get started by **creating a new repl, repo, or any code space.**.

:::tip
<Linkto>[replit.com](https://replit.com)</Linkto> is reccomended for a started codespace
:::

## Tutorial Environment Setup

You need to start with a new node/javascript project, and when you have that up, you can create a folder called `tests`. After you've done that, in your package.json file, add

``` json 
"scripts": {
  "test": "node tests/mytest.js"
}
```

When you've done that, in your tests folder, put a file called `mytest.js` and put the following into it: 
``` javascript
var test = require('chitchatsjs')
```
Now you can run `npm run test` in your terminal to run tests!

**Huzzah**! You've set up a proper test enviorment for ChitChatjs! 

Now you can go on and use your new enviorment to learn some ChitChatjs! Let's go!
