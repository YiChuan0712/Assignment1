[link to README.md](./README.md)

# Markdown
Markdown is a simple syntax that formats text as headers, lists, boldface, and so on.


  * [1 Paragraphs and Line Breaks](#1-paragraphs-and-line-breaks)
  * [2 Headers](#2-headers)
  * [3 Blockquotes](#3-blockquotes)
  * [4 Lists](#lists)
  * [Code Blocks](#code-blocks)
  * [Horizontal Rules](#horizontal-rules)
  * [Table](#table)
  * [Links](#links)
  * [Images](#images)



### 1 Paragraphs and Line Breaks

#### 1.1 Paragraphs

***
Code:

    This is 
    the first paragraph. 
    
    This is the second paragraph.

Preview:

This is 
the first paragraph.
    
This is the second paragraph.
***

#### 1.2 Line Breaks

***
Code:

    This is 
    the first paragraph.

Preview:

This is 
the first paragraph.
***




### 2 Headers

#### 2.1 Setext
***
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

***
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





### Lists

#### Unordered
***
Code:

    *   Yichuan
    *   Yichuan
    *   Yichuan
Preview:
*   Yichuan
*   Yichuan
*   Yichuan

***





#### Ordered
***
Code:

    1.  Yichuan
    2.  Yichuan
    3.  Yichuan
Preview:

1.  Yichuan
2.  Yichuan
3.  Yichuan

***

#### Indented

##### Blockquote
To put a blockquote within a list item, the blockquote’s > delimiters need to be indented:

Code:

    *   A list item with a blockquote:

        > This is a blockquote
        > inside a list item.
Preview:
***
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

***
##### Code Block
To put a code block within a list item, the code block needs to be indented twice — **8 spaces** or **two tabs**:

Code:

    *   A list item with a code block:

            <code goes here>
Preview:
***
*   A list item with a code block:

        <code goes here>

***
##### Nested List
Code:

    * A
      * A1
      * A2
    * B
    * C
Preview:
***
* A
  * A1
  * A2
* B
* C

***
### Code Blocks
HTML Tag: `<pre>`

Indent every line of the block by at least **4 spaces** or **1 tab**.

Code:

    This is a normal paragraph:

        This is a code block.
Preview:
***
This is a normal paragraph:

    This is a code block.
***
A code block continues until it reaches a line that is not indented (or the end of the article).

Within a code block, ***ampersands (&)*** and angle **brackets (< and >)** are automatically converted into HTML entities.

Code:

        <div class="footer">
            &copy; 2004 Foo Corporation
        </div>
Preview:
***
    <div class="footer">
        &copy; 2004 Foo Corporation
    </div>
***
Following sections Fenced Code Blocks and Syntax Highlighting are extensions, you can use the other way to write the code block.
#### Fenced Code Blocks
Just wrap your code in ```` ``` ```` (as shown below) and you won't need to indent it by four spaces.

Code:

    Here's an example:

    ```
    function test() {
      console.log("notice the blank line before this function?");
    }
    ```
Preview:
***
Here's an example:

```
function test() {
  console.log("notice the blank line before this function?");
}
```
***
#### Syntax Highlighting
In your fenced block, add an optional language identifier and we'll run it through syntax highlighting ([Support Languages](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)).

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
### Horizontal Rules
HTML Tag: `<hr />`
Places **three or more hyphens (-), asterisks (*), or underscores (_)** on a line by themselves. You may use spaces between the hyphens or asterisks.

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
### Table
HTML Tag: `<table>`

It's an extension.

Separates column by **pipe (|)** and header by **dashes (-)**, and uses **colon (:)** for alignment.

The outer **pipes (|)** and alignment are optional. There are **3 delimiters** each cell at least for separating header.

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
***
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
