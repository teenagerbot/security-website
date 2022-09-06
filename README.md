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
