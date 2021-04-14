[link to README.md](./README.md)

# Markdown
Markdown is a simple syntax that formats text as headers, lists, and so on.


  * [1 Paragraphs and Line Breaks](#1-paragraphs-and-line-breaks)
  * [2 Headers](#2-headers)
  * [3 Blockquotes](#3-blockquotes)
  * [4 Lists](#4-lists)
  * [5 Code Blocks](#5-code-blocks)
  * [6 Horizontal Rules](#6-horizontal-rules)
  * [7 Tables](#7-tables)
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
***
This is 
the first paragraph.
    
This is the second paragraph.
***

#### 1.2 Line Breaks


Code:

    This is     
    the first paragraph.

Preview:
***
This is       
the first paragraph.
***




### 2 Headers

#### 2.1 Setext

Code:

    This is an H1
    =============
    This is an H2
    -------------

Preview:
***
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
***
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
***
> This is 
> the first paragraph.
> This is the first paragraph.
> 
> This is the second paragraph.
> This is the second paragraph.

***





### 4 Lists

#### 4.1 Unordered

Code:

    *   Yichuan
    *   Yichuan
    *   Yichuan
Preview:
***
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
***
1.  Yichuan
2.  Yichuan
3.  Yichuan

***


### 5 Code Blocks

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
### 7 Tables

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
