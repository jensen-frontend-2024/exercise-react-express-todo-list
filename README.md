# Todo List

In this exercise I want you to create a todo list with React, express.js and Sqlite. The todo list is will be simple, not any fancy functionalities or animations _(unless you relly want to get creative)_.

## Instructions

### Setup

You will need a SQLite database that can be connected to you express backend. The requests from the React frontend should go to the express backend that in turn gets the data from the SQLite DB and sends it back to the client (React frontend).

### Basics

- A view/page _( React Router )_ to display all the todos.

- A view/page that has a form where you can add new todos. The new todo should be saved to the DB straight away and then the user must be navigated to the view/page that displays the todos.

- You should should be able to be mark a todo as completed

- You should be able to remove a todo. When you remove a todo, the todo must be deleted from the DB as well.

- If you do a hard refresh, or loose internet connection, the todos must persists. In other words, you should always fetch the todos from the DB.

- Styling is important in frontend development, don't neglect that. But a piece of advice, do the styling part or the logic part first, don't do them at the same time. On thing at a time.

### More complexity

- An author and timestamp should be visible on every todo.

- You should be able to edit a todo. Create a new view/page for editing a specific todo. This page should not be visible on a navbar, it can only be reached if editing a specific todo.

- You should be able to sort the todos after timestamp or author. Timestamp should be the default sorting.

  <details>
  <summary>Hint..</summary>

  Use ORDER BY in your sql query.
  </details>

## Extra stuff that you can use.

### Google fonts

[Google fonts - Docs & Catalog](https://fonts.google.com/)

Browse the fonts, in order to use one in your application follow these steps:

1. Click on a font you like, [`Roboto`](https://fonts.google.com/specimen/Roboto) for instance.

2. Click the `Get font`-button and then the `Get embeded code`-button.

3. Make sure you're in the `Web`-tab and click on the `@import`-radio button

4. Cope the code inside the style-tags to the top of you css file and add the font-family to your html-tag

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

html {
  font-family: 'Roboto', serif;
}
```

This will set the default font-family on all the elements inside the html-tag. If you want a different font-family on certain elements you can just add those in different css-selectors.

### Material Icons

[Material icons - Docs & Catalog](https://fonts.google.com/icons)

Browse the icons, in order to use them in your application follow these steps:

1. Copy this code and add it inside the head-tag on your HTML document.

```js
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" rel="stylesheet" />
```

2. Pick an icon by clicking on it. A side meny should come in from the right.

3. Make sure you are on the `Web`-tab, scroll down to "Inserting the icon".

4. Copy the code and add it in your HTML document or your generated HTML code inside your js-files. Here is an example for a home icon:

```html
<span class="material-symbols-outlined"> home </span>
```

The class is what gives the icon its looks, and it comes from the link-tag you added earlier. The text "home" is the reference to the icon that is being retrieved from material icons.

Remember, that icons can be styled, you can change color and such things. You usually need some flex-styling on the parent element in order to be properly align the icon with the rest of the content inside the parent element.
