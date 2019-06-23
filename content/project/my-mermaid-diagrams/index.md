---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Project: TEST A"
summary: "Testing HUGO Academic Projects making and management"
authors: ["dbj"]
tags: ["test"]
categories: ["test-category"]
date: 2019-06-23T04:01:37+02:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

diagram: true
---

## Diagrams
You can generate diagrams and flowcharts from text, in a similar manner as Markdown.

Just add 

      diagram: true 

to a page’s YAML front matter and insert your Mermaid diagram syntax in the Diagram shortcode and that’s it. For example
```html
                    { {< diagram >}}
                    graph TD;
                        A[Wake up] -->|go to the kitchen| B(Open the cofee can)
                        B --> C{Plastic or metal spoon?}
                        C -->|Plastic spoon| D[A bit more coffee]
                        C -->|Metal   spoon| E[A bit less coffee]
                    { {< /diagram >}}
```
{{< diagram >}}
graph TD;
    A[Wake up] -->|go to the kitchen| B(Open the cofee can)
    B --> C{Plastic or metal spoon?}
    C -->|Plastic spoon| D[A bit more coffee]
    C -->|Metal   spoon| E[A bit less coffee]
{{< /diagram >}}

## Code highlighting

### C++

```cpp
#include <string>
#include <iostream>

int main() {
  string nam("dbj") ;
    for ( auto && c : name )
       cout << endl << c ;
}
```

| option              | type    | description                 | config.toml | preamble |
| ------------------- | ------- | --------------------------- | ----------- | -------- |
| highlight           | boolean | enable/disable highlighting | yes         | yes      |
| highlight_languages | slice   | choose additional languages | yes         | yes      |
| highlight_style     | string  | choose a highlighting style | yes         | yes      |

## Twitter
To include a single tweet, pass the tweet’s ID from the tweet’s URL as parameter to the shortcode:

      { {< tweet 1142324187207540737 >} }

{{< tweet 1142324187207540737 >}}