**Task 0: Early Styling**

- Create a new directory `css_basic` in the repository `alx_html_css`
- Copy into this directory the `index.html` and `tweets.html` that you created in the `html_basic` directory of the [previous project](https://savanna.alxafrica.com/rltoken/FrPtBW-FheYIwWHE75yyIQ):
- Create an empty `styles.css`.
- Create the file `base.css` and set the content of this [file](https://savanna.alxafrica.com/rltoken/tA17nawbm6cOABq3COTLnw)

In each of your HTML files, add these 2 lines within the `<head>` tag (do not confuse with the `<header>` tag!):

```
<link href="base.css" rel="stylesheet">
<link href="styles.css" rel="stylesheet">
```

If you refresh your webpages in your browser, they should now look a bit better!

We just told your webpages to use the CSS rules described in those two files, and to apply them to your HTML code.

---

##### Task 1. Positioning

Even though each element of your webpages now has a different style, you may notice they still are stacked on top of each other, and that’s probably not what you want. CSS brings a few different approaches to positioning that one may use depending on cases.

For this project, we’re going to use CSS Flexbox, a recent set of CSS properties that work with recent browsers.

Our goal is to get a layout that looks like this:

| Content of the `<header>` tag  |                              |
| ------------------------------ | ---------------------------- |
| Content of the `<article>` tag | Content of the `<aside>` tag |
| Content of the `<footer>` tag  |                              |

As a reminder, there are also two container tags playing critical roles here:

- `<main>` contains the area that includes `<article>` and `<aside>`.
- `<body>` contains all of them together.

Here are steps to get this layout, which you will have to write as CSS code in the `styles.css` file:

- Both container tags, `<body>` and `<main>` must be told that they are containers to flexible boxes: you need to apply the `display: flex` property to both of them.
- However, `<body>` contains a column of three boxes (`<header>`, `<main>` and `<footer>`), therefore you must apply the flex-direction: column property to `<body>`; whereas `<main>` contains a row of 2 boxes (`<article>` and `<aside>`), so you must apply the `flex-direction: row` property to `<main>`.
- Ensure the `<main>` tag keeps an automatic height and width, by applying the `flex: auto` property to it.
- To wrap up the layout, you want to be sure that your content (article) takes ⅔ of the width of the page, and your aside takes ⅓; you can assign to them the number of boxes they should fill in. This is done by applying the property `flex: 2` to `<article>` (using up 2 boxes), and `flex: 1` to `<aside>` (using up 1 box).
- Finally, you want to be sure that the user can scroll within your `<article>` and your `<aside>`. You can do this by applying the `overflow-y: auto` CSS property to both of them.

If you’ve done all of those properly, and your HTML structure is correct, you should get exactly the layout we were trying to get.

Do note that the exact rendering you’re getting may be slightly different depending on your browser (namely, about whether header and footer are fixed or not when the user scrolls), but should always match the layout presented above.

---

##### Task 2. Responsive web design

You may notice that the website keeps this layout when you make your browser window smaller, or visit it from a smartphone, and it’s unpleasant to use that way for your users. No worries, we covered this for you: just add the attribute `class="works_on_smartphone"` on the `<body>` tag in your `index.html` file, and the layout you just created will degrade nicely as you resize the window!

But you’ll notice, if you visit your website on a smartphone, that it will still have that layout, and just seem “zoomed out”. That’s because you need to adjust what is called the “viewport” of the browser when rendering the page.

```
Hint: this gets done by adding a certain tag to your HTML code.
```

**NB: Do well to thoroughly go through the base css file that was provided to you to understand exactly which styles produces which result.**

---

##### Task 3. Some more styling

Your website is unique, and if you want it not to look like everyone else’s, you may want to take some time to style everything of it as you wish!

What you’re allowed to do:

- You may add any non-positioning-related CSS rules to `styles.css` (like colors, backgrounds, borders, …)
- You may do whatever you want with the HTML content and the CSS that applies inside the `<article>` tag.
- You may add a logo to the top-left of your page. To keep it simple, rather than use an image, feel free to use a unicode character, [from this table](https://savanna.alxafrica.com/rltoken/mCun37Y6BDMmcuPwP3jumQ) for instance. One way to make it work: add a first item in the list in your `<header>`, before all other list items, and just put the HTML-code for the character in it (it starts with “&” and ends with “;”). To make it look like a logo, if you want the character to be bigger, you can add the `class="logo"` attribute on the
- tag, we added the CSS rule for you.

**What you’re not allowed to do:**

- Do not change the layout strategy, done with CSS Flexbox, as described above. Feel free to experiment with positioning within the `<article>` tag if you wish; but please refrain to do so anywhere else.

  ---

  