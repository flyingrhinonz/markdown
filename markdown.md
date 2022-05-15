Yet another markdown cheat sheet.
This one separates the basic markdown (supported everywhere)
from the advanced markdown (which is supported to varying levels by different programs).
I'm not including markdown features that are site-specific with the goal that this
page only covers what you'd expect to find everywhere (almost).


# Basic markdown:


Headings:
======

# Heading 1

Heading 1
==

## Heading 2

Heading 2
--

### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

####### Seven hashes (heading 6 prefixed with one hash)
######## Eight hashes (heading 6 prefixed with two hashes)

Paragraphs:
====

This is regular text in a
paragraph. Just a block of lines
one after the other. One or more empty lines separate paragraphs.


And a second paragraph here. This is caused by
one or more empty lines above.

How to force a line break?  
Simply end a line  
with two or more spaces.
This is where vim kenmode comes in handy - to show trailing whitespace.


Horizontal rules:
======

Three or more of any of these:  - _ *  will cause a horizonal line:

---

Same as:
___

Same as:

***


Lists:
======

List items can begin with:  *  , -  , +  it doesn't really matter:

* List item 1
* List item 2
* List item 3
- List item 4
+ List item 5

A regular line here to end the list above and start a new list below (otherwise lists get merged):

- List item 1
- List item 2
- List item 3

Another regular line and a list using;  +  for items:

+ List item 1
+ List item 2
+ List item 3


A numbered list begins with a number. Any number:

1. Item 1
2. Item 2
2. 1984\. This is a number and a dot. Need to escape the dot to prevent it from detection by the list mechanism.
2. Item 3
1. Item 4

Which number - doesn't really matter:

1. Item 1
    1. Item 1.1
    1. Item 1.2
1. Item 2
1. Item 3


Another list example:

1. Item 1
* Item 2
* Item 3
1. Item 4


Using points within a list:

1. Item 1
    * Point 1
    * Point 2
        * Point 2a
        * Point 2b
            * Point 2b1
            - Point 2b2 (* - +  prefix doesn't matter)
            + Point 2b3
1. Item 2
    - Point 1
    - Point 2
    * Point 3
        * Point 3a
1. Item 3
    + Point 1
    + Point 2


Emphasis:
======

This text is *italic* .

This text is _italic_ .

This text is **bold** .

This text is __bold__ .

This text is ***bold and italic*** .

This text is ___bold and italic___ .

This text is **_bold and italic_** .

This text is ~~strikethrough~~ . Advanced - not supported everywhere.

This text is ==highlight== . Advanced - not supported everywhere.

This text is `inline code` . Depending upon your viewer - it may or may not be highlighted.

And this is how to display `` `backticks` `` . Escape it with double backticks.


Paragraphs:
====

Regular quoting:

> This text is quoted.

More quoting:

>> This text is even more quoted.
It is multiline too  
and the trailing double space trick
works here too.

Yet more quoting:

>>> Additional level of quoting here.

Nested quotes:

> This quote is top level.
>> And this quote is nested.

Multi paragraph:

> This as a multiple  
paragraph quoting example.
>
> Second paragraph here. It shares the same quoting as the first paragraph.  
Note how the empty line between paragraphs also includes the:  >  which
basically continues the quoting.

->This text is center paragraph. Advanced - not supported everywhere.<-

-> This multi line paragraph is  
also center paragraph.  
The double space end trick works here too.
Advanced - not supported everywhere.<-


Links:
====

Really good guide to markdown: [here](https://itsfoss.com/markdown-guide/)

The link description text goes in: [...] and the actual webpage link goes in: (...) . BTW - the link above actually points to a good markdown tutorial.


Automatic links:
Use: <...> to surround a real email or web URL and it becomes a working link:

<ken@example.com>

<http://www.example.com>



Images:
======

![image_desc](file:///C:/Work/image.png "opt_title")

![descriptive text](./images/image.jpg)

Image links begin with:  !  . Put a description of the image inside the: [...]  and a link to the image inside the: (...) .


# Advanced markdown:

This may not be supported everywhere.


Tables:
======

Pretty format:

|Title 1  | Title 2  |
|---------|----------|
| Line 1a | Line 1b  |
| Line 2a | Line 2b  |

This less pretty format works too:

Title 1 | Title 2 | Title 3
--- | --- | ---
Blah1 | **Blah2 text** | `blah3`


Code blocks:
======

Code block follows:

```
This is
a block
of code.
Also displayed in monospace font.
```


Definitions:
======

Some item.
: This is a definition of some item.

Blah
: Definition of blah. Can be
spread over multiple lines.  
The trick of double space at the end to force line break works here too.

Third term
: Definition of third term. Empty lines above don't matter.


Footnotes:
======

Footnote example [^1] . See bottom of page for footnote text.

[^1]: This is the content of the footnote and link: [blah](http://example.com)


Checklists:
======

- [x] Checkbox item checked
- [ ] Unchecked


