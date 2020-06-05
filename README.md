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

```c
copy("\u2800")
```

# log

<img width="350" src="https://user-images.githubusercontent.com/66380341/83735092-dce64e80-a68a-11ea-8654-f2952cb6a938.PNG">

  200b doesn't work.
  
<img width="450" src="https://user-images.githubusercontent.com/66380341/83899173-eeb31900-a792-11ea-9222-283c821ddebc.PNG">

