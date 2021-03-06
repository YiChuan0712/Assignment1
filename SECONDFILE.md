[link to README.md](./README.md)

# a Simple Markdown Guideline
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

End a line with **two or more spaces**.

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

    H1 Sized Header
    =============

    H2 Sized Header
    -------------

Preview:
***
H1 Sized Header
=============

H2 Sized Header
-------------
***




#### 2.2 atx

Code:

    # H1 Sized Header
    ## H2 Sized Header
    ###### H6 Sized Header

Preview:
***
# H1 Sized Header
## H2 Sized Header
###### H6 Sized Header
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
    #include <iostream>
    
    int main()
    {
      std::cout << "Hello World!" << std::endl;
      return 0;
    }
    ```
Preview:
***

```
#include <iostream>

int main()
{
  std::cout << "Hello World!" << std::endl;
  return 0;
}
```
***
#### 5.2 Syntax Highlighting
Code:

    ```c++
    #include <iostream>
    
    int main()
    {
      std::cout << "Hello World!" << std::endl;
      return 0;
    }
    ```
Preview:
***
```c++
#include <iostream>

int main()
{
  std::cout << "Hello World!" << std::endl;
  return 0;
}
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
| S             | A             | T             | O             | R             |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| A             | R             | E             | P             | O             |
| T             | E             | N             | E             | T             |
| O             | P             | E             | R             | A             |
| R             | O             | T             | A             | S             |

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
| S             | A             | T             | O             | R             |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| A             | R             | E             | P             | O             |
| T             | E             | N             | E             | T             |
| O             | P             | E             | R             | A             |
| R             | O             | T             | A             | S             |

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

### 8 Links

Code:

    [a link to an external web site](https://www.baidu.com/)
Preview:
***
[a link to an external web site](https://www.baidu.com/)

***
### 9 Images

Code:

    an image that is a file in the directory
    ![img](./image.jfif)

    an image that is located on the web
    ![img](https://www.baidu.com/img/flexible/logo/pc/result@2.png)
Preview:
***
an image that is a file in the directory
![img](./image.jfif)

an image that is located on the web
![img](https://www.baidu.com/img/flexible/logo/pc/result@2.png)
***
