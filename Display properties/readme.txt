1. display properties

a) block 
answer -> The `display: block;` CSS property is used to define an element as a block-level element. Here's what it does:

1. **Starts on a New Line:** Elements with `display: block;` start on a new line in the layout of the web page. They create a "block" that takes up the full width available in their parent element.

2. **Stretches Full Width:** Block-level elements automatically stretch horizontally to fill the entire width of their parent container. You can set their width to a specific value if you want to control their horizontal size.

3. **Allows Setting Width and Height:** You can explicitly set the width and height of a block-level element using CSS properties like `width` and `height`.

4. **Accepts Margin and Padding:** You can apply margins and padding to block-level elements. Margins control the space outside the element, while padding controls the space inside the element's border.

5. **Can Contain Inline and Other Block Elements:** Block-level elements can contain other block-level elements, inline elements, and text. They create a new "block" context for the elements inside them.

Examples of block-level elements include `<div>`, `<p>`, `<h1>` to `<h6>`, `<ul>`, `<ol>`, and many others. When you apply `display: block;` to an inline element (like a `<span>`), it changes the element to a block-level element, altering its layout behavior as described above.

b) Inline
answer -> 
The `display: inline;` CSS property is used to define an element as an inline element. Here's what it means and how it behaves:

1. **Inline Elements:**
   - **No Line Breaks:** Inline elements do not start on a new line. They flow within the content and do not break the flow of the document. Multiple inline elements can appear next to each other on the same line.
  
   - **Only Takes Up Necessary Width:** Inline elements only take up as much width as necessary. They do not stretch to the full width of their parent container. For example, an inline element with a small amount of text will only be as wide as the text it contains.

   - **Height and Width Cannot Be Set:** Unlike block elements, you cannot set a specific height or width for inline elements. These properties do not affect inline elements. However, you can set padding and margin, which will apply horizontally (left and right) but not vertically (top and bottom).

   - **Examples of Inline Elements:** `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, `<input>`, etc.

Here's an example of how `display: inline;` is used in CSS:

```css
span {
    display: inline;
    background-color: lightblue;
    padding: 10px;
    margin: 5px;
}
```

In this example, all `<span>` elements on the webpage will be displayed inline, meaning they will appear on the same line as much as possible, and their background color, padding, and margin properties will be applied horizontally without affecting the vertical layout.

c) inline-block
answer -> 
The `display: inline-block;` CSS property value combines aspects of both block-level and inline elements. When you set an element's display property to `inline-block`, it behaves like an inline element in terms of how it flows in a line with surrounding content, but it also allows you to set width, height, margin, and padding values, just like block-level elements.

Here's what `display: inline-block;` does:

1. **Inline Behavior:**
   - **Flows Inline:** Elements with `display: inline-block;` do not start on a new line. They flow within the text or other inline elements, allowing content to flow around them horizontally.

2. **Block Behavior:**
   - **Size Properties:** You can set width, height, margin, and padding. This means you have control over the size of the element.
   - **Box Model:** Respects the CSS box model, allowing you to specify padding and margin values, affecting the space around the element.
   - **Alignment:** You can use properties like `text-align` to align inline-block elements horizontally within their parent element.

This combination of inline flow and block-level styling makes `display: inline-block;` very useful for creating components like navigation menus, where elements need to be in a line horizontally (like inline elements) but also need to have specific widths, heights, and spacing (like block-level elements).

Example:

```css
.inline-block-element {
    display: inline-block;
    width: 100px;
    height: 50px;
    margin: 10px;
    padding: 5px;
    background-color: lightblue;
    text-align: center;
    line-height: 50px;
}
```

In the above example, the element with the class `inline-block-element` will be an inline-block element. It will have a width of 100 pixels, a height of 50 pixels, a margin of 10 pixels around it, and a padding of 5 pixels inside it. It will be horizontally centered within its parent element due to `text-align: center;` and vertically centered due to `line-height: 50px;`.

d) none
answer -> 
The `display: none;` CSS property is used to hide an element from the web page entirely. When applied to an element, it removes the element from the normal document flow, meaning it won't take up any space and won't affect the layout of other elements on the page. Essentially, the element becomes invisible and inaccessible.

Here's an example of how you might use `display: none;` in CSS:

```css
.hidden-element {
    display: none;
}
```

In this case, any HTML element with the class `hidden-element` will not be displayed on the web page when the CSS is applied.

This property is commonly used in scenarios where you want to toggle the visibility of an element based on user interaction, for example, when creating dropdown menus, modal dialogs, or tabs. JavaScript can be used to manipulate the CSS property value and change an element's visibility dynamically.

/**

Certainly! Here's a list of CSS `display` property values, along with explanations of each value:

1. **`block`**: 
   - The element generates a block-level container box, which means it starts on a new line and stretches the full width of its containing element.
   - You can set width, height, margin, and padding for block-level elements.

2. **`inline`**: 
   - The element generates an inline-level box, which means it does not start on a new line and only takes up as much width as necessary.
   - You cannot set width and height for inline elements, and margin/padding only affect the left and right sides.

3. **`inline-block`**: 
   - The element generates an inline-level block container, which means it behaves like an inline element but allows you to set width, height, margin, and padding.

4. **`none`**: 
   - The element is not displayed on the web page. It is completely removed from the document flow and cannot be interacted with.

5. **`flex`**: 
   - The element generates a flex container, enabling a flex context for its direct children. You can use flexbox layout properties on the children elements.

6. **`grid`**: 
   - The element generates a grid container, enabling a grid context for its direct children. You can use grid layout properties on the children elements.

7. **`table`**: 
   - The element generates a block-level table container, which behaves like a `<div>` but can be used to create a table structure using CSS properties like `table-row` and `table-cell`.

8. **`table-row`**: 
   - The element behaves like a `<tr>` element in an HTML table. It's used inside a `display: table;` element to create table rows.

9. **`table-cell`**: 
   - The element behaves like a `<td>` element in an HTML table. It's used inside a `display: table-row;` element to create table cells.

10. **`table-header-group`**, **`table-footer-group`**, **`table-row-group`**: 
    - These values are used to define the layout behavior of rows in specific sections of a table when using `display: table;`.

11. **`inherit`**: 
    - The element inherits the `display` property from its parent element.

12. **`initial`**: 
    - The element is displayed according to its default value, which is typically `inline` for most elements.

13. **`unset`**: 
    - The element is displayed according to the inherited value if one exists, otherwise, it behaves like `initial`.

Each of these values determines how an element is displayed on the web page and how it interacts with other elements in the document flow.
**/


