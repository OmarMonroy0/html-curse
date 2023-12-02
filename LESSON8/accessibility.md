# ACCESSIBILITY  

In this lesson we will see how to make our web site accessible for everyone


### ACESSSIBILITY TREE

This tree is similar to the DOM one but this contains information for accessibility 

Each node in this tree contains 4 elements:

* Names
* Description
* role
* state

### PROCESSS OF ELEMENTS FROM HTML TO USER

<center>
    <img src="./accesibily-tree.png" src="accessibility tree"/>
</center>
 

As we can see in the image the first process of the elements in html is to pass through the DOM tree after that the elements go through 2 parts; the first one is the User Interface and the second one is Accessibility tree 

The accessibility tree is created  from the DOM tree and kept in sync with it. Assistive technlogies such as screen readers interact with the accessibility tree rather than directly with the DOM.

### MAIN USAGE

This tree is really important to allow accessibility and experience of users with some disabilities 

This tree is the representation of the structure of a web page that centers in the information and characteristics that are important for any kind of user 



### HOW TO GET A WEB PAGE FOR ALL USERS

* Use descriptive content, labels and alt atributes
* Use semantic gropu elements (this helps a lot the tree )
* Test keyboard controlls: Add some shorcuts with the keyboard to navigate easier
  

### WAI-ARIA 

The "Web Accessibility Initiative - Accessible Rich Internet Applications" specification  for accessible HTML created by the World Wide Web Consortium (W3C). Oftentimes just referred to as just ARIA, it contains  a set of HTML  attributes that can be added to provide extra information to the accessibility tree


### ARIA ATRIBUTES

They are usually grouped into three main categories:

* **Roles**.- What the element is doing,  used to define the purpose of the element. These can be broken in more subgroups
  1. **Landmark:** Major content areas, navigational landmarks.
  2. **Structure**: Document structure information.
  3. **Widget**: Interactive Elements.
  4. **Window**: sub-windows in the browser
  5. **Live Region**: Regions with dynamically changing content.
* **Properties**: Extra meaning and characteristcs of the element, such as labels.
* **States**: current state of the element, such as if it disabled or not.


### LANDMARK ROLES (Reference point)


En HTML, una "landmark" (punto de referencia) es una región específica de una página web que se utiliza para identificar y proporcionar una navegación más fácil y accesible para los usuarios. Las landmarks son elementos HTML con roles específicos que ayudan a los usuarios, especialmente aquellos que utilizan tecnologías de asistencia, a comprender y navegar la estructura de la página web de manera más eficiente.

Some elements that can act like a landmark are:

1. header
2. nav
3. main
4. aside
5. footer
6. section
7. article
8. form

We can also crete a landmark by adding the attribute role

An element of HTML with the a specific  attribute "role" that provides extra semantic information about the element ( this elements are grouping elements and represent an entire section of the web page).

<header role="banner">
    <h1>Logotipo de la Empresa</h1>
    <nav role="navigation">
        <ul>
            <li><a href="/">Inicio</a></li>
            <li><a href="/productos">Productos</a></li>
            <li><a href="/contacto">Contacto</a></li>
        </ul>
    </nav>
</header>

```html
<header role="banner">
    <h1>Logotipo de la Empresa</h1>
    <nav role="navigation">
        <ul>
            <li><a href="/">Inicio</a></li>
            <li><a href="/productos">Productos</a></li>
            <li><a href="/contacto">Contacto</a></li>
        </ul>
    </nav>
</header>
```
<footer role="contentinfo">
    <p>&copy; 2023 Mi Empresa. Todos los derechos reservados.</p>
    <p><a href="/privacidad">Política de Privacidad</a></p>
</footer>

```html
<footer role="contentinfo">
    <p>&copy; 2023 Mi Empresa. Todos los derechos reservados.</p>
    <p><a href="/privacidad">Política de Privacidad</a></p>
</footer>
```

```html
<div rol ="banner">
        <h1> My accessible Web Page </h1>
</div>
```

this are the first elements that are going to be seen by the user in the web page.

### STRUCTURE ROLES

Document structural information 

This are really similar to the last one but with smaller elements such as lists , table etc, in the same way the use the attribute role to give the usage.


### WIDGET ROLES.

These roles are for interactive elements such as tab,searchbox, button 

<div role="button">
    Click Me
</div>

### WINDOW ROLES 

They are subwindows in the browser
Examples:

- dialog
- alertdialog

<div role ="dialog" aria-labelledby = "title">
    <h2 id="title"> Succesfully saved changes </h2>
    <button> Dissmis </button>
</div>


### LIVE REGION ROLES

This elements will be checked periodically by the assitant technology of the web page to inform the user of any changes on the content, this areas contain information  that is relevant for the user and that change without need  that the user make specific actions