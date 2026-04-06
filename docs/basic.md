# Fennec Basic Styling

Fennec styling involves defining styles for text prior to the text:

(large,weight:bold) Hello World

Compiled into HTMl (depending on compiler and settings) would be:

```HTML
<span style="font-size: 2em; font-weight: bold">Hello World</span>
```

Inline styling is also possible by wrapping inline text in the % operator,
signifying that it should be treated separately (while keeping parent text styles unless overidden)

(large) Hello %(weight:bold) World%

Would compile into:

```HTML
<span style="font-size: 2em;">Hello <span style="font-weight:bold">World</span></span>
```

Multi-line styling involves using square brackets to show which lines inbetween an open and closed bracket to style

Therefore
(large)\[
Hello
World
]
Compiles into

```HTML
<div style="font-size:2em;">
    <span>Hello</span>
    <br>
    <span>World</span>
</div>
```
