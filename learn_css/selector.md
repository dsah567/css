# selector 
A CSS selector is the first part of a CSS Rule. It is a pattern of elements and other terms that tell the browser which HTML elements should be selected to have the CSS property values inside the rule applied to them.

## Types of selectors

### Type selectors target an HTML element
`h1 {   }`

### Class selectors target an element that has a specific value for its class attribute:
`.box { }`

### ID selectors target an element that has a specific value for its id attribute:
`#unique {  }`

### Attribute selectors
This group of selectors gives you different ways to select elements based on the presence of a certain attribute on an element:
`a[title] { }`

Or even make a selection based on the presence of an attribute with a particular value:
`a[href="https://example.com"]{ }`

| Selector | Example | Description|
|----------|---------|------------|
|[attr]	|a[title]	|Matches elements with an attr attribute (whose name is the value in square brackets).
|[attr=value]	|a[href="https://example.com"]	|Matches elements with an attr attribute whose value is exactly value — the string inside the quotes.
|[attr~=value]	|p[class~="special"]	|Matches elements with an attr attribute whose value is exactly value, or contains value in its (space separated) list of values.
|[attr|=value]	|div[lang|="zh"]	|Matches elements with an attr attribute whose value is exactly value or begins with value immediately followed by a hyphen.


### Pseudo-classes and pseudo-elements
This group of selectors includes pseudo-classes, which style certain states of an element. 
`a:hover {  }`
```css
:first-child
:last-child
:only-child
:invalid
:hover
:focus
:visited
:active
:nth-child
```

It also includes pseudo-elements, which select a certain part of an element rather than the element itself.
`p::first-line {    }`

#### Combinators
The final group of selectors combine other selectors in order to target elements within our documents. The following, for example, selects paragraphs that are direct children of <article> elements using the child combinator (>):
`article > p {  }`

The next-sibling combinator (+)
The child combinator (>)

If you want to select siblings of an element even if they are not directly adjacent, then you can use the subsequent-sibling combinator (~). To select all \<img> elements that come anywhere after \<p> elements, we'd do this:
`p ~ img`