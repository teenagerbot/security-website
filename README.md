# security-website
this library will help protect your site from embedding on other people's sites

This library is designed to protect your site from embedding on other people's sites, that is, other programmers will not be able to embed your site on their own through <iframe>

How to use

We connect the file:
```<script src="https://blocking.teleweb.repl.co/secure.min.js" link-block="block.html" secure is-file></script>```

Where:
```link-block``` - file that will be displayed when your site is blocked

```is-file``` - checks if the file you linked in the attribute exists *link-block*

If it exists, it reproduces it in an iframe, otherwise it displays its default version of the page

```secure``` - enables blocking, if you do not register it, then it does not block in the iframe

attention

you should connect the script tag ONLY in the head

![зображення](https://JSLearn.teleweb.repl.co/img/ф.png)

If you connect it to another place or the parent of the script is not a head, it will give an error:

![зображення](https://JSLearn.teleweb.repl.co/img/a.png)

![зображення](https://JSLearn.teleweb.repl.co/img/b.png)

Example:
```(https://link..../hi.html)```:

```
<html>
  <head>
    <title>example</title>
    <link rel="stylesheet" href="example.css">
    <script src="https://blocking.teleweb.repl.co/secure.min.js" link-block="block.html" secure is-file></script>
  </head>
  <body>
    <h1>hello I'm website</h1>
  </body>
</html>
```

Now let's imagine that another programmer has received your site's link and is trying to embed your site for himself:

```
<html>
  <head>
    <title>example hacker</title>
    <link rel="stylesheet" href="exampleHacker.css">
  </head>
  <body>
    <iframe src="https://link..../hi.html" width="90%" height="50%"></iframe>
  </body>
</html>
```

Result:
![зображення](https://JSLearn.teleweb.repl.co/photos/1662483761081.gif)

File block.html does not exist, so the program issued its own version of the inscription

Attention: never make your site in the editor codepen.io - protection does not work (apparently the editor itself removes the restrictions)

Looking at your browser language, the program displays text in your language
