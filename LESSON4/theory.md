# MOST COMMON TAGS USED IN HTML 

1.  ###  Paragraphs
```html
    <p> Used for block of text</p>
```
2. ### Headings

```html
    <h1> Principal Heading</h1>
    <h2> Second Heading</h2>
    <h3> Third Heading</h3>
    <h4> </h4>
    <h5> </h5>
    <h6> </h6>
```

3. ### Images

```html
    <img src="here comes url" alt="we place here an alternative text to show while the the image is loading">
```

4. ### LISTS WITH NO ORDER

```html
    <ul>
        <li> First Element</li>
        <li> Second Element </li>
        <li> Third Element </li>
    </ul>
```

5. ### LISTS WITH ORDER

```html
    <ol>
        <li> First Element</li>
        <li> Second Element </li>
        <li> Third Element </li>
    </ol>
```
For this kind of list we can set some attributes to define the order of the elements 


```html
    <ol type ="i">
        <li> First Element</li>
        <li> Second Element </li>
        <li> Third Element </li>
    </ol>
```

will produce 

i. First Element
ii. Second Element
iii. Third Element
iv. Four Element



```html
    <ol type ="4">
        <li> First Element</li>
        <li> Second Element </li>
        <li> Third Element </li>
    </ol>
```

will produce 

4. First Element
5. Second Element
6. Third Element
7. Four Element


```html
    <ol type ="a">
        <li> First Element</li>
        <li> Second Element </li>
        <li> Third Element </li>
    </ol>
```
will produce 

a. First Element

b. Second Element

c. Third Element

d. Four Element


IMPORTANT NOTE: We can create nested lists.

### Paragraphs with line break in the browser

```html
    <pre>
        This is like a paragraph however it shows line breaks in the browser and the common paragraph
        does not
    </pre>
```

###  Line break for tag common paragraphs

```html
    <p>
       Hi <br />
       How are you <br />
    </p>
```

### Horizontal Rule ----------------------------------

```html
    <p>
        Part 1
    </p>
    <hr />
    <p>
        Part 2
    </p>
    <hr />
```

### LINK TO ANOTHER PAGES

```html
    <a href="https://algoexpert.io"> Algo Expert</a>
```

For this tag "Algo Expert" is the text shown instead od the link but at clicking the name we will be redirected, href is an attribute and it uses another atributes not insted of openning in another tab to do it in another window.

```html
    <a href="https://algoexpert.io" target="_self"> Algo Expert</a>

    <a href="https://www.ejemplo.com" target="_blank">Abrir en una nueva ventana</a>
```

###  Rendering italic and black letters

```html
    <p><strong>NOTE: </strong> <em>This is italic </em></p>
```

<nav>
    <ul>
        <li> <a href = "https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p"> Paragraph</a>
    </ul>
</nav>

As you can see we are using nav to encapsulate all the links, that is the main function of nav.