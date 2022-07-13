# CSS Concepts

## Basics

- You can add style to an element by specifying it in the `style` element and setting a property for it like this:

  ```css
  element {
    property: value;
  }
  ```

- You can add the same group of styles to many elements by creating a list of selectors. Each selector is separated with commas like this:

  ```css
  selector1,
  selector2 {
    property: value;
  }
  ```

- Since there will be many more styles, it's best to put all the styles in a separate file and link to it.
- Now you need to link the `css` file so the styles will be applied again. Nest a self-closing `link` element in the `head` element. Give it a `rel` attribute value `stylesheet` and an `href` attribute value of the css file.
- For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a `meta` element with a special `content` attribute.

  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  ```

- The `div` element is used mainly for design layout purposes unlike the other content elements you have used so far.
- Comments in CSS look like this:

  ```css
  /* comment here */
  ```

- So far you have been using type selectors to style elements. A class _selector_ is defined by a name with a dot directly in front of it, like this:

  ```css
  .class-name {
    styles
  }
  ```
