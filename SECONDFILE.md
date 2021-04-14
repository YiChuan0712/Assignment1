[link to README.md](./README.md)

# Markdown
Markdown is a simple syntax that formats text as headers, lists, and so on.


  * [1 Paragraphs and Line Breaks](#1-paragraphs-and-line-breaks)
  * [2 Headers](#2-headers)
  * [3 Blockquotes](#3-blockquotes)
  * [4 Lists](#4-lists)
  * [5 Code Blocks](#5-code-blocks)
  * [6 Horizontal Rules](#6-horizontal-rules)
  * [7 Table](#7-table)
  * [8 Links](#8-links)
  * [9 Images](#9-images)


***

### 1 Paragraphs and Line Breaks
    
#### 1.1 Paragraphs

Code:

    This is 
    the first paragraph. 
    
    This is the second paragraph.

Preview:

This is 
the first paragraph.
    
This is the second paragraph.
   

#### 1.2 Line Breaks


Code:

    This is 
    the first paragraph.

Preview:

This is 
the first paragraph.
***




### 2 Headers
***
#### 2.1 Setext

Code:

    This is an H1
    =============
    This is an H2
    -------------

Preview:

This is an H1
=============

This is an H2
-------------
***




#### 2.2 atx

Code:

    # This is an H1
    ## This is an H2
    ###### This is an H6

Preview:

# This is an H1
## This is an H2
###### This is an H6
***


### 3 Blockquotes
***
Code:

    > This is 
    > the first paragraph.
    > This is the first paragraph.
    > 
    > This is the second paragraph.
    > This is the second paragraph.
Preview:
> This is 
> the first paragraph.
> This is the first paragraph.
> 
> This is the second paragraph.
> This is the second paragraph.

***





### 4 Lists
***
#### 4.1 Unordered

Code:

    *   Yichuan
    *   Yichuan
    *   Yichuan
Preview:
*   Yichuan
*   Yichuan
*   Yichuan

***





#### 4.2 Ordered

Code:

    1.  Yichuan
    2.  Yichuan
    3.  Yichuan
Preview:

1.  Yichuan
2.  Yichuan
3.  Yichuan

***


### 5 Code Blocks
***
#### 5.1 Fenced Code Blocks
Code:
    ```
    function test() {
      console.log("notice the blank line before this function?");
    }
    ```
Preview:
***
```
function test() {
  console.log("notice the blank line before this function?");
}
```
***
#### 5.2 Syntax Highlighting
Code:

    ```ruby
    require 'redcarpet'
    markdown = Redcarpet.new("Hello World!")
    puts markdown.to_html
    ```
Preview:
***
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
***

### 6 Horizontal Rules
Code:

    * * *
    ***
    *****
    - - -
    ---------------------------------------
    ___
Preview:
***
* * *
***
*****
- - -
---------------------------------------
___
***
### 7 Table

Code:
```
| Left | Center | Right |
|:-----|:------:|------:|
|aaa   |bbb     |ccc    |
|ddd   |eee     |fff    |

 A | B 
---|---
123|456


A |B 
--|--
12|45
```

Preview:

| Left | Center | Right |
|:-----|:------:|------:|
|aaa   |bbb     |ccc    |
|ddd   |eee     |fff    |

 A | B 
---|---
123|456

A |B 
--|--
12|45
***
## Span Elements
### Links
HTML Tag: `<a>`

Markdown supports two style of links: inline and reference.

#### Inline
Inline link format like this: `[Link Text](URL "Title")`

Title is optional.

Code:

    This is [an example](http://example.com/ "Title") inline link.
    
    [This link](http://example.net/) has no title attribute.
Preview:
***
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.
***
If you’re referring to a local resource on the same server, you can use relative paths:

Code:

    See my [About](/about/) page for details. 
Preview:
***
See my [About](/about/) page for details. 
***
#### Reference
You could predefine link references. Format like this: `[id]: URL "Title"`

Title is also optional. And the you refer the link, format like this: `[Link Text][id]`

Code:

    [id]: http://example.com/  "Optional Title Here"
    This is [an example][id] reference-style link.
Preview:
***
[id]: http://example.com/  "Optional Title Here"
This is [an example][id] reference-style link.
***
That is:

* Square brackets containing the link identifier (**not case sensitive**, optionally indented from the left margin using up to three spaces);
* followed by a colon;
* followed by one or more spaces (or tabs);
* followed by the URL for the link;
* The link URL may, optionally, be surrounded by angle brackets.
* optionally followed by a title attribute for the link, enclosed in double or single quotes, or enclosed in parentheses.

The following three link definitions are equivalent:

Code:

    [foo]: http://example.com/  "Optional Title Here"
    [foo]: http://example.com/  'Optional Title Here'
    [foo]: http://example.com/  (Optional Title Here)
    [foo]: <http://example.com/>  "Optional Title Here"
Uses an empty set of square brackets, the link text itself is used as the name.

Code:

    [Google]: http://google.com/
    [Google][]
Preview:
***
[Google]: http://google.com/
[Google][]
***
### Emphasis
HTML Tags: `<em>`, `<strong>`

Markdown treats **asterisks (*)** and **underscores (_)** as indicators of emphasis. **One delimiter** will be  `<em>`; **double delimiters* will be `<strong>`.

Code:

    *single asterisks*

    _single underscores_

    **double asterisks**

    __double underscores__
Preview:
***
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__
***
But if you surround an * or _ with spaces, it’ll be treated as a literal asterisk or underscore.

You can backslash escape it:

Code:

    \*this text is surrounded by literal asterisks\*
Preview:
***
\*this text is surrounded by literal asterisks\*
***
### Code
HTML Tag: `<code>`

Wraps it with **backtick quotes (`)**.

Code:

    Use the `printf()` function.
Preview:
***
Use the `printf()` function.
***
To include a literal backtick character within a code span, you can use **multiple backticks** as the opening and closing delimiters:

Code:

    ``There is a literal backtick (`) here.``
Preview:
***
``There is a literal backtick (`) here.``
***
The backtick delimiters surrounding a code span may include spaces — one after the opening, one before the closing. This allows you to place literal backtick characters at the beginning or end of a code span:

Code:

    A single backtick in a code span: `` ` ``

    A backtick-delimited string in a code span: `` `foo` ``
Preview:
***
A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``
***
