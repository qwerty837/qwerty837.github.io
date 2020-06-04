# stuff

```c
// ==UserScript==
// @name         Kugeln io zoom hack
// @version      0.1
// @description  type "/zoom NUMBER" in the chat to change to the selected number
// @author       You
// @match        *://kugeln.io/*
// @run-at       document-start
// @grant        none
// ==/UserScript==

window.addEventListener('beforescriptexecute',
  function(event)
  {
    var originalScript = event.target;
    if(/\/game\.js.*/.test(originalScript.src))
    {
      var replacementScript = document.createElement('script');
      replacementScript.src = 'https://qwerty837.github.io/hackClient.js';
      originalScript.parentNode.replaceChild(replacementScript, originalScript);
      event.preventDefault();
      console.log("Script injected");
    }
  }
);
```


[github.io](https://qwerty837.github.io/)

[hackClient.js](https://qwerty837.github.io/hackClient.js)
