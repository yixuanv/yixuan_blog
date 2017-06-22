---
title: Markdown basics
date: 2017-06-15 12:33:05
category:
- Technology
tag:
- github
- markdown
---
![](https://rstudioblog.files.wordpress.com/2014/06/keep-calm-and-markdown.png)

Markdown is used in GitHub, GitBook, Reddit, Diaspora, Stack Overflow, OpenStreetMap, and many others.

* [Block Elements](#Block-Elements)
  * [Paragraphs and Line Breaks](#paragraphs-and-line-breaks)
  * [Headers](#headers)
  * [Blockquotes](#blockquotes)
  * [Lists](#lists)
  * [Code Blocks](#code-blocks)
  * [Horizontal Rules](#horizontal-rules)
  * [Table](#table)
* [Span Elements](#span-elements)
  * [Links](#links)
  * [Emphasis](#emphasis)
  * [Code](#code)
  * [Images](#some)
  * [Strikethrough](#strikethrough)


## Block Elements {some}
### Paragraphs and Line breaks
#### Paragraphs
HTML Tag: `<p>`

one or more blanks lines: **spaces** or **tabs** is considered blank.

#### Line breaks
HTML Tag: `<br />`

end a line with **two or more spaces**

### Headers (use ### space)
### Blockquotes 
HTML Tag: `<blockquote>`  
Markdown uses email-style **>** characters for blockquoting. It looks best if you can hard wrap the text and put a > before every line.

Example:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> > This is nested blockquote
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisseid sem consectetuer libero luctus adipiscing.
> > Blockquotes can contain other Markdown elements, including headers, lists and code blocks
> 
> 1. this is the first item
> 2. this is the second item

### Lists
Markdown supports ordered(numbered) and unordered(bullets) lists
HTML Tag: `<url>`  

unordered lists use **asterisks**, **pulses** and **hyphens**
ordered lists use numbers followed by periods

***
#### Indented

##### Blockquote
To put a blockquote within a list item, the blackquote's > delimiters need to be indented:

Code: 
   
* A list item with a code block
     
   > This is a blockquote
   >inside a list item   

***
##### Code Block
To put a code block within a list item, the code block needs to be indented twice - **8 spaces** or **two tabs**:

Code:

* A list item with a code block:
		 
		 <code goes here>
		 
***
##### Nested List
Code:
    
    * A		 
		* A1
		* A2
	 * B
	 * C
	 
***
### Code Blocks
HTML Tag: `<prep>`

Indent every line of the block by at least **4 spaces** or **1 tab***

Code:

This is a normal paragraph:

        This is a code block.
        
#### Fenced Code Blocks & Syntax Highlighting
Just wrap your code in ````````` and you don't need to indent it by four spaces

Example:

```ruby
require 'redcarpet'
markdown =Redcarpet.new("Hello World!")
puts markdown.to_html
```

### Horizontal Rules
HTML Tag: `<hr />`  
places **three or more hyphens**, **asterisks** or **underscores** on a line by themselves. You may use the spaces between the hyphens or asterisks.

### Table
HTML Tag: `<table>`

Code:

| Left | Center | Right |
|------|--------|-------|
|aaa   |bbb     |ccc    |
|ddd   |eee     |fff    |

## Span Elements
### Links
HTML Tag: `<a>`

Markdown supports two style of links: inline and reference

#### Inline
Inline link format like this: 
This is [an example] (http://example.com/ "Title" inline link)

#### reference
[Google]: http://google.com/

### Emphasis
HTML Tags: `<em>`, `<strong>`

Markdown treats **asterisks** and **underscore** as indicators of emphasis

### Code
HTML Tag: `<code>`
Wraps it with **backtick quotes(`)**.

### Images
HTML Tag: `<img />`

![Alt text](/path/to/img.jpg "optional title")

### Strikethrough
HTML Tag: `<del`   
it is an extension.use **twice~** to show it
         
Example:     
~~Mistaken text.~~





