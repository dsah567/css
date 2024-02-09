# Parts of a box
Making up a block box in CSS we have the:

- Content box: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
- Padding box: The padding sits around the content as white space; size it using padding and related properties.
- Border box: The border box wraps the content and any padding; size it using border and related properties.
- Margin box: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.

```html
.box {
  box-sizing: border-box;
  width: 350px;
  inline-size: 350px;
  height: 150px;
  block-size: 150px;
  margin: 10px;
  border: 5px solid black;
}
```
To turn on the alternative model for an element, set box-sizing: border-box on it:
No need to add up the border and padding to get the real size of the box.