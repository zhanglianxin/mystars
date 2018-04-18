# mystars

> Organize my starred repos.
>
> ```javascript
> (() => {
>     let text = '';
>     let titles = document.querySelectorAll('h3');
>     let descs = document.querySelectorAll('div.py-1');
>     for (let i = 0; i < titles.length; i++) {
>         text += `### [${titles[i].innerText}](${titles[i].querySelector('a').href})\n`;
>         if (descs[i].childNodes.length > 1) {
>             text += descs[i].querySelector('p[itemprop="description"]').innerText + '\n';
>         }
>     }
>     
>     console.log(text);
> })();
> ```
