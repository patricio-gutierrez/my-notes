# HTML Concepts

## Basics

### Tags

- HTML elements have opening tags like `<h1>` and closing tags like `</h1>`.
- When elements have multiple attributes, the order of the attributes doesn't matter.

### Headers

- The `h1` to `h6` heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so `h2` elements have less importance than `h1` elements. **Only use one `h1` element per page** and place lower importance headings below higher importance headings.
- When you add a lower rank heading element to the page, it's implied that you're starting a new subsection.

### Paragraphs

- The `p` element is used to create a paragraph of text on websites.

### Comments

- Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.

### SEO & Accessibility

- HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.
- Indenting nested elements two more spaces than their parent element improves readability.

### Images

- You can add images to your website by using the `img` element. `img` elements have an opening tag without a closing tag. A tag for an element without a closing tag is known as a _self-closing tag_.
- HTML _attributes_ are special words used inside the opening tag of an element to control the element's behavior. The `src` attribute in an `img` element specifies the image's URL (where the image is located).
- All `img` elements should have an `alt` attribute. The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.
- The `figure` element represents self-contained content and will allow you to associate an image with a caption.
- A figure caption (`figcaption`) element is used to add a caption to describe the image contained within the `figure` element.

### Links

- You can link to another page with the anchor (a) element. For example, `<a href='https://freecodecamp.org'></a>` would link to `freecodecamp.org`.
- A link's text must be placed between the opening and closing tags of an anchor (`a`) element. For example, `<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>` is a link with the text `click here to go to freeCodeCamp.org`.
- Add a `target` attribute with the value `_blank` to the anchor (`a`) element's opening tag, so that the link opens in a new tab.
- Before adding any new content, you should make use of a `section` element to separate the content from the future content.

### Lists

- To create an unordered list you can use the tag `ul`.
- To create an ordered list you can use the tag `ol`.
- To create a list element you can use the tag `li`.

### Text Decoration

- Emphasize the word element by wrapping it in an emphasis `em` element.
- The `strong` element is used to indicate that some text is of strong importance or urgent.

### Forms

- Now you will add a web form to collect information from users using the tag `form`.
- The `action` attribute indicates where form data should be sent. For example, `<form action="/submit-url"></form>` tells the browser that the form data should be sent to the path `/submit-url`.
- The `input` element allows you several ways to collect data from a web form. Like `img` elements, `input` elements are _self-closing_ and do not need closing tags.
- There are many kinds of inputs you can create using the `type` attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.
- In order for a form's data to be accessed by the location specified in the `action` attribute, you must give the text field a `name` attribute and assign it a value to represent the data being submitted.
- Placeholder text is used to give people a hint about what kind of information to enter into an input.
- To prevent a user from submitting your form when required information is missing, you need to add the `required` attribute to an `input` element. There's no need to set a value to the `required` attribute. Instead, just add the word `required` to the `input` element, making sure there is space between it and other attributes.
- Use the `button` element to create a clickable button. For example, `<button>Click Here</button>` creates a button with the text `Click Here`. The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's `action` attribute.
- Both `input` and `button` elements are inline elements, which don't appear on new lines.
- You can explicitly add the `type` attribute with the value `submit`.
- You can use **radio buttons** for questions where you want only one answer out of multiple options.
- `label` elements are used to help associate the text for an `input` element with the input element itself (especially for assistive technologies like screen readers).
- To make it so selecting one radio button automatically deselects the other, both buttons must have a `name` attribute with the same value.
- If you select the radio button and submit the form, the form data for the button is based on its `name` and `value` attributes. Since your radio buttons do not have a `value` attribute, the form data will include `name=on`, which is not useful when you have multiple buttons.
- The `fieldset` element is used to group related inputs and labels together in a web form. `fieldset` elements are _block-level_ elements, meaning that they appear on a new line.
- The `legend` element acts as a caption for the content in the `fieldset` element. It gives users context about what they should enter into that part of the form.
- Forms commonly use _checkboxes_ for questions that may have more than one answer.
- There's another way to associate an `input` element's text with the element itself. You can nest the text within a `label` element and add a `for` attribute with the same value as the `input` element's `id` attribute.
- Like radio buttons, form data for selected checkboxes are `name` / `value` attribute pairs. While the `value` attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.
- In order to make a checkbox checked or radio button selected by default, you need to add the `checked` attribute to it. There's no need to set a value to the `checked` attribute. Instead, just add the word `checked` to the `input` element, making sure there is space between it and other attributes.

### Id's

- The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other `id` values for the entire page.

### Head

- All page content elements that should be rendered to the page go inside the `body` element. However, other important information goes inside the `head` element.
- The `title` element determines what browsers show in the title bar or tab for the page.
- The entire contents of the page are nested within an `html` element. All other elements must be descendants of this `html` element.
- Add the `lang` attribute with the value `en` to the opening `html` tag to specify that the language of the page is English.
- All pages should begin with `<!DOCTYPE html>`. This special string is known as a _declaration_ and ensures the browser tries to meet industry-wide specifications.
- You should allow people to use their native language. Tell the browser to encode multiple languages by adding a `meta` element as a child of the `head` element. Set its `charset` attribute to `UTF-8`.
