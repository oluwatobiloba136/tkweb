---
template: blog_comment.html
title: My Blog Features test
description: This page is to demostrate great features and extension that can be incorporate in my blog.
date: 2022-04-17
hide:
  - navigation
  # - toc
tags: 
  - new
---

Creating a branded static site from a set of Markdown file to host a blog is actually a fun to me. <br>
With the use of ***[Material for MkDocs](https://squidfunk.github.io/mkdocs-material//)*** blogging become pretty easy, 

<p hidden>#more</p>

### Abbreviation
!!! example

The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

### Admonition
!!! info inline

    Lorem ipsum dolor sit amet, consectetur
    adipiscing elit. Nulla et euismod nulla.
    Curabitur feugiat, tortor non consequat
    finibus, justo purus auctor massa, nec
    semper lorem quam in massa.

Important: admonitions that use the inline modifiers must be declared prior to the content block you want to place them beside. If there's insufficient space to render the admonition next to the block, the admonition will stretch to the full width of the viewport, e.g. on mobile viewports.

<br>

### Content Tabs
!!! example
=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```
### Button

[Send :fontawesome-solid-paper-plane:](#){ .md-button }

### Code block

``` py hl_lines="2 3" linenums="1" title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

### Data Table

| Method      | Description                          |
| ----------- | ------------------------------------ |
| `GET`       | :material-check:     Fetch resource  |
| `PUT`       | :material-check-all: Update resource |
| `DELETE`    | :material-close:     Delete resource |


### Sequence Diagram 

``` mermaid
sequenceDiagram
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```


### State Diagram
``` mermaid
stateDiagram-v2
    state if_state <<choice>>
    [*] --> IsPositive
    IsPositive --> if_state
    if_state --> False: if n < 0
    if_state --> True : if n >= 0
```

### Class Diagram
``` mermaid
classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```

### ERD diagram

``` mermaid
erDiagram
  CUSTOMER ||--o{ ORDER : places
  ORDER ||--|{ LINE-ITEM : contains
  CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```


### Formatting
- ==This was marked==
- ^^This was inserted^^
- ~~This was deleted~~

**Keyboard keys: **
++ctrl+alt+del++

**Sub- and Superscripts: ** <br>
  - H~2~0
  - A^T^A


### Task List
!!! info "CRISP-DM"
- [x] Business Understanding
- [x] Data Understanding
- [ ] Data Preparation
    * [x] Select data
    * [x] Clean data
    * [ ] Integrate data
- [ ] Modeling
- [ ] Evaluation
- [ ] Deployment



<!-- Footer for blog post -->
