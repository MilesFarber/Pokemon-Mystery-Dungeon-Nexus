---
layout: default
---
# Hi, this is a Markdown header

This is text.
This is text one linebreak below. It will appear on the same line.

This is text TWO linebreaks below. It will NOT appear on the same line.

~~This is striked text, using two tildes, delet this.🔫~~

*This is italic text, using one asterisk.*

_You can also use one underscore._

**This is bold text, using two asterisks.**

*This is italic, but you can add **two asterisks to turn the italic bold, and end both with three asterisks.***

*~~You can do the same~~ in reverse, and **even** in between.*

> This is a quote, using a GreaterThan sign.

<sub>Smol text at the bottom using HTML subscript tags.</sub>

<sup>Smol text at the top using HTML superscript tags.</sup>

<!- Use HTML comment tags to make something invisible. This is visible because there's only one dash instead of two. ->

<!-- Bruh. -->

Type some [LaTeX](https://en.wikibooks.org/wiki/LaTeX/Mathematics) between dollar signs to display math expressions. $\sqrt{3x-1}+(1+x)^2$

Use two dollar signs to display a math block. Here's the Cauchy-Schwarz Inequality.

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

1. Use a number, a dot, and a space
2. To make an ordered list.

* Use an asterisk and a space
* To make an unordered list.

- You can also use
- A dash and space instead.

1. You can use 1
1. For every row
1. To allow Markdown
1. To number the list
1. Automatically.

* Use tabs
  * To add layers
    * To the unordered list.

[ ] Square brackets with a space in between creates a checkbox.
[x] Replace the space with a lowercase x to mark the checkbox.

Asterisk, space, asterisk, space, asterisk...
* * *
...creates a horizontal rule.

| Head 1 | Head Two |
| --- | --- |
| Use vertical bars to create a table. | Use monospace fonts to avoid confusion. |
| Cells can vary in width | And do not need to be perfectly aligned within columns. |
| There must be at least three hyphens | In each column of the header row. |

| Beginning | Both | End |
| :--- | :---: | ---: |
| Add colons as described above | To tell the text | Where to align |

<details><summary>This is a Collapse with a Label.</summary>
<p>
To create a Collapse, use the HTML tag `details`, then `p`, then `/p`, then `/details`, between LessThan and GreaterThan signs.
To add a Label to the collapse, add the HTML tags `summary` and `/summary` on the right of the `details` HTML tag.
</p>
</details>

`Use grave accents for tiny code or keywords.`

Putting HEX codes such as `#9933FF` or `rgb(153, 51, 255)` between grave accents displays a color.

```js
// Use three grave accents and the language to create code blocks. Here's some meme js.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```md
Specify md or no language to display normal text. Long lines outside of code blocks wrap around, but long lines inside code blocks do not. This is a long enough text to demonstrate this. Did you know that in terms of Human to Pokemon breeding Vaporeon is- ok sorry.
```

Specify math if you really, really hate dollar signs.

```math
\sqrt{-1}
```

[It even supports Mermaid Flowcharts!](https://mermaid-js.github.io/mermaid)

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

Also GeoJSON and TopoJSON!

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```

```topojson
{
  "type": "Topology",
  "transform": {
    "scale": [0.0005000500050005, 0.00010001000100010001],
    "translate": [100, 0]
  },
  "objects": {
    "example": {
      "type": "GeometryCollection",
      "geometries": [
        {
          "type": "Point",
          "properties": {"prop0": "value0"},
          "coordinates": [4000, 5000]
        },
        {
          "type": "LineString",
          "properties": {"prop0": "value0", "prop1": 0},
          "arcs": [0]
        },
        {
          "type": "Polygon",
          "properties": {"prop0": "value0",
            "prop1": {"this": "that"}
          },
          "arcs": [[1]]
        }
      ]
    }
  },
  "arcs": [[[4000, 0], [1999, 9999], [2000, -9999], [2000, 9999]],[[0, 0], [0, 9999], [2000, 0], [0, -9999], [-2000, 0]]]
}
```

As if that wasn't enough, you can even use ASCII STL 3D models.

```stl
solid cube_corner
  facet normal 0.0 -1.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 1.0 0.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
  facet normal 0.0 0.0 -1.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 1.0 0.0 0.0
    endloop
  endfacet
  facet normal -1.0 0.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 0.0 1.0
      vertex 0.0 1.0 0.0
    endloop
  endfacet
  facet normal 0.577 0.577 0.577
    outer loop
      vertex 1.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
endsolid
```

By default, https://pages.github.com/ automatically creates links from HTTPS URL's.

Github commits are shortened. https://github.com/FlarosOverfield/Zeitgeist/commit/ae19d2dc3aca4d4aefd0e9d35484645ca69f7201 

To customize the link, put the name of the link between square parentheses, then put the link between round parentheses, with no spaces.

[This is a link to another local Markdown page.](./index.md)

[This is a link to another webpage.](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

[You can link files too. If the file can't display on a browser window, a download will start.](https://static.f-list.net/images/avatar/tokumei%20kii.png)

Add ! at the beginning before the square parenthesis to embed. This is a smol image one line below.
![Possum](https://static.f-list.net/images/avatar/tokumei%20kii.png)

This is a l o r g e image two lines below.

![Bigger Possum](https://static.f-list.net/images/charinline/a0/ce/a0ceb589e437b739a897f116d9e9065a62d338bf.png)

Embedded files cannot be bigger than 10MB, and must be either .PNG, .JPG, .SVG, .LOG, .DOCX, .PPTX, .XLSX, .TXT, .PDF, .ZIP, or .GZ.
Animated files such as .GIF, .MP4, or .MOV, will only embed properly on Desktop (x86) Chromium and Firefox.

## This is a smaller header

### An even smaller header

#### so smol

##### pls halp

###### a

You can use footnotes with a caret and a number, between square brackets[^1].
You can also use whatever name you want instead of a number.[^Name]

[^1]: Add a colon (NOT semicolon) to invoke the footnote, make sure it's at the bottom of the page and at the beginning of the line.
[^Name]: Although it will still display as a number with certain themes.
