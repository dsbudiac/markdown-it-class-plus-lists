Plugin classes bullet lists defined with plus signs only. To allow for special css treatment (or whatever).

# Usage

```js
const md = require('markdown-it')()
  .use(require('markdown-it-class-plus-lists'), className);
```

`className` is "checklist" by default.

# Markdown

```markdown
+ List item 1
+ List item 2
+ List item 3

- Bullet 1
- Bullet 2
```

# Output

```html
<ul class="checklist">
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ul>

<ul>
  <li>Bullet 1</li>
  <li>Bullet 2</li>
</ul>
```