# Lecture 0 - HTML, CSS

### Specificity in CSS (check [style.html](style.html))
1. inline
2. id
3. class
4. type

### Selectors (see [attribute.html](attribute.html))
|       |                           |
|-------|---------------------------|
| a, b  | Multiple Element Selector |
| a b   | Descendant Selector       |
| a > b | Child Selector            |
| a + b | Adjacent Sibling Selector |
| [a=b] | Attribute Selector        |
| a:b   | Pseudoclass Selector      |
| a::b  | Pseudoelement Selector    |

### Responsive design
- Viewport (e.g. proper responsive behavior in mobiles with: `<meta name="viewport" content="width=device-width, initial-scale=1">`)
- Media Queries (see [responsive.html](responsive.html))
- Flexbox (see [flexbox.html](flexbox.html))
- Grids (check [grid.html](grid.html))

### [Bootstrap](https://getbootstrap.com/)
Bootstrap is a powerful, feature-packed frontend toolkit. Build anything—from prototype to production—in minutes.

Check [hello.html](hello.html)

### [SASS](https://sass-lang.com/)
Stylesheet language that’s compiled to CSS.
It allows you to use variables, nested rules, mixins, functions, and more, all with a fully CSS-compatible syntax.
Sass helps keep large stylesheets well-organized and makes it easy to share design within and across projects.

Check [variables.html](variables.html), compile [variables.scss](variables.scss) with:

`sass --watch variables.scss variables.css`

and run [variables.html](variables.html):

`start variables.html`





