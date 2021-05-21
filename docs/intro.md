---
sidebar_position: 1
---

# Tutorial Intro

Let's discover **ChitChatjs in less than 5 minutes**.

## Getting Started

Get started by **creating a new repl, repo, or any code space.**.

:::tip
[replit.com](https://replit.com) is reccomended for a started codespace
:::

## Tutorial Environment Setup

Please run the following in your terminal:
``` shell
npm i -g chitchatsjs
```

And when you have that up, you can create a folder called `tests`. After you've done that, in your package.json file(at the root of your repo), add

``` json 
{
  "scripts": {
    "test": "npx chitchatsjs node tests/mytest.chit.js && node tests/mytest.chit.js"
  }
}
```

Now when you've done that, in your tests folder, put in a file called `mytest.chit.js`. 


**Horray!**

Now that you have setup your enviorment, you can now start writing some ChitChatjs!