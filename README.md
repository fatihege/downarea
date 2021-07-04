![DownArea Logo](https://imgupload.io/images/2021/07/04/downarea-500x200.png "DownArea Logo")

---

# DownArea
An easy to use, lightweight and extensible JavaScript markdown editor library.

---

> CDN Links
> > https://cdn.jsdelivr.net/gh/fatihege/downarea@1.0.0/src/downarea.min.js
> > https://cdn.jsdelivr.net/gh/fatihege/downarea@1.0.0/src/downarea.min.css
> 
> > https://cdn.jsdelivr.net/gh/fatihege/downarea@1.0.0/src/downarea.js
> > https://cdn.jsdelivr.net/gh/fatihege/downarea@1.0.0/src/downarea.css

---

## Tools

| Key         | Name             |
|        ---: | :---             |
| heading     | Headings         |
| bold        | Bold             |
| italic      | Italic           |
| bold-italic | Bold Italic      |
| link        | Links            | 
| image       | Image            |
| blockquote  | Blockquote       |
| u-list      | Unordered List   |
| o-list      | Ordered List     |
| sl-code     | Single Line Code |
| code-block  | Code Block       |

---

## Simple Usage

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>DownArea</title>
    <link rel="stylesheet" href="downarea.min.css">
</head>
<body>

<div class="editor"></div>

<script src="downarea.min.js"></script>
<script>
    var downarea = new DownArea({
        elem: document.querySelector('.editor'), // Required - Container element
        resize: DownArea.RESIZE_BOTH, // Optional - RESIZE_OFF | RESIZE_VERTICAL | RESIZE_HORIZONTAL | RESIZE_BOTH
        hide: ['heading'], // Optional - Type the keys of the tools you want to hide here.
    });
</script>
</body>
</html>
```

---

## Tool Methods (Public Methods)

| Tool Key    | Method                           | Args          |
| ----------- | -------------------------------- | ------------- |
| heading-1   | `.addHeading(level: number = 1)` | *default (1)* |
| heading-2   | `.addHeading(level: number = 1)` | 2             |
| heading-3   | `.addHeading(level: number = 1)` | 3             |
| heading-4   | `.addHeading(level: number = 1)` | 4             |
| heading-5   | `.addHeading(level: number = 1)` | 5             |
| heading-6   | `.addHeading(level: number = 1)` | 6             |
| bold        | `.addBold()`                     | *empty*       |
| italic      | `.addItalic()`                   | *empty*       |
| bold-italic | `.addItalic()`                   | *empty*       |
| normal-link | `.addLink(type: number = 0)`     | *default (0)* |
| quick-link  | `.addLink(type: number = 0)`     | 1             |
| email       | `.addEmail()`                    | *empty*       |
| image       | `.addImage()`                    | *empty*       |
| blockquote  | `.addBlockquote()`               | *empty*       |
| u-list      | `.addUnorderedList()`            | *empty*       |
| o-list      | `.addOrderedList()`              | *empty*       |
| sl-code     | `.addSingleLineCode()`           | *empty*       |
| code-block  | `.addCodeBlock()`                | *empty*       |
