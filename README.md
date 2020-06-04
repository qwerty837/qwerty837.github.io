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
copy("\u200B")
```

# log

<img width="450" src="https://user-images.githubusercontent.com/66380341/83735092-dce64e80-a68a-11ea-8654-f2952cb6a938.PNG">
<img width="450" src="https://user-images.githubusercontent.com/66380341/83735098-de177b80-a68a-11ea-8912-485d16f36b3d.PNG">
