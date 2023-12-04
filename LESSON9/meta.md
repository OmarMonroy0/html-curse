# META TAGS

## Definition

This is a HTML tag used for providing extra metadata about webpage. Most of them will use a name and content pair for the type of metadata  and its value.

## MOST COMMON META TAGS.

### CHARSET

```html
<meta charset="utf-8">
```

It is used in html to declare the character encoding for the document  which is a way of representing and interpreting characters in a computer by using utf-8 we ensure of using all characteres in the Unicode character set

#### UTF-8

Stands for Unicode Trasnformation  Format 8-bit is a character encoding standard which is an universal character encoding that aims to represent every character from every writing system in the World and its really popular because of its efficiency, backward compatibility with ASCII..


### SIZE OF THE SCREEN

```html
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

It is used in html to provide instructions  to the browser about how to control the page's dimension and scalling on diffenrent devices.

This is particularly important for creating  a responsive  design  that adapts well to various screen sizes and resolutions.

* **width=device-width:** This setting instructs the browser to set the width of the viewport to the width of the device. This ensures that the content fits well within the device's screen width.

* **initial-scale=1.0:** This setting sets the initial zoom level when the page is first loaded. A value of 1.0 means that the page is displayed at its initial size without any zooming.


### AUTHOR

```html
    <meta name = "author" content="author's name" />
```

This meta tag is used to set the name of the web page's author.

### DESCRIPTION

```html
    <meta name = "descripcion" content="small description of the web page" />
```

### REDIRECTING PAGE AFTER x SECONDS

```html
<meta http-equiv="refresh" content="3;url=https://www.mozilla.org" />
```
It will redirect the page automatically after just 3 seconds to the link.


## FAVICON

Stands for favorite icon and will include the icon for the web page which is the smal image left to the name of the tab.

<center>
    <img src="./favicon.png" alt ="favicon"/>
</center>


```html
    <link rel = "icon" href="favicon.png" />
```
## BASE.

```html
    <!-- This line goes in the head -->
    <base href="https://algo"/>

    <!-- this would go to https://algo/frontend -->

    <a href="/frontend"> Frontend </a>
```

This is used to save the main page or the root and not being repeating the same content every time, is something similar to what I do with postman using {{url}}