# FORMS

to create forms in html we use

```html
    <body>
        <form>
            <label for="username">  User </label>
            <input id = "username" type="text" />

            <label for="password"> Password </label>
            <input id ="password" type = "password" />

        </form>
    </body>
```

In this html code we can see label points to an exactly one element that is the reason to set an id to each input


### PLACEHOLDER

```html
    <body>
        <form>
            <label for="username">  User </label>
            <input id = "username" type="text" placeholder = "user123" />

            <label for="password"> Password </label>
            <input id ="password" type = "password" />

        </form>
    </body>
```

placeholder is used to set some text in the input field while there is no text written by the user in the field input


<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" />
 </form>

#### code 

```html
<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" />
 </form>
```

### Adding some basic constraints

<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
 </form>

#### code 

```html
<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
 </form>

```
Now the user should inpunt a password of at least length 6


### Adding a submit button

<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
 </form>

#### Code
```html
<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
 </form>
```

As you can  see we write 2 ways to make a submit button, the first one is by using input type = "submit" or  by using 

```html
    <button> Button name </button>
```

### input Date

<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type="date">
 </form>

#### Code
```html
<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type="date">
 </form>
```

 ### Input checkbox

 <form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type = "checkbox" />

 </form>

This allows to create a square or any figure you decide where the user can click and in that way to mark that input

#### Code
```html
 <form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type = "checkbox" />

 </form>
```

### Radio button input

 <form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type = "checkbox" />
    <fieldset>
        <legend> Choose your favorite animal<legend>
        <label for="dog">Dog</label>
        <input id="dog" type="radio" name="animal" value="dog">
        <label for="cat"> Cat </label>
        <input id="cat" type="radio" name="animal" value="cat" />
        <label for="bird"> Bird </label>
        <input id="bird" type="radio" name="animal" value="bird"/>
    </fieldset>
 </form>


```html
<form>
    <label for="username">  User </label>
    <input id = "username" type="text" placeholder = "user123" />
    <label for="password"> Password </label>
    <input id ="password" type = "password" placeholder = "place in here your password" minlength="6" />
    <input type="submit" />
    <button> Submit </button>
    <input type = "checkbox" />
    <fieldset>
        <legend> Choose your favorite animal<legend>
        <label for="dog">Dog</label>
        <input id="dog" type="radio" name="animal" value="dog">
        <label for="cat"> Cat </label>
        <input id="cat" type="radio" name="animal" value="cat" />
        <label for="bird"> Bird </label>
        <input id="bird" type="radio" name="animal" value="bird"/>
    </fieldset>
 </form>
```

As you can see in this case we place  all the radio inputs in a fieldset which is also a semantic grouping tag and legend is to give a name to that fieldset

