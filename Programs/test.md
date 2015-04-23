Markdown test
=============

This is a test for Markdown capabilities.

# Header 1 (don't use!)
## Header 2 (used in Table of Contents)
### Header 3
#### Header 4
##### Header 5
###### Header 6

This sentence has some *emphasis*, and it also **embiggens** the smallest man.

I like to use greater than > or less than < symbols.

~~Mistaken text.~~

Here is some cool `monospaced` text.

This is an image!
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

## Columns

Extended markdown for layout purposes.

### Two Column layout

[row start]
[col start]
First column
[col end]
[col start]
Second column
[col end]
[row end]

### Three Column Layout
[row start]
[col start]
First column
[col end]
[col start]
Second column
[col end]
[col start]
Third column
[col end]
[row end]

### Four Column Layout
[row start]
[col start]
First column
[col end]
[col start]
Second column
[col end]
[col start]
Third column
[col end]
[col start]
Fourth column
[col end]
[row end]

### Empty Columns
[row start]
[col start]
[col end]
[col start]
Second column
[col end]
[col start]
Third column
[col end]
[col start]
[col end]
[row end]

### Multi Row Columns
[row start]
[col start]
[col end]
[col start]
Second column
[col end]
[row end]
[row start]
[col start]
First column
[col end]
[col start]
[col end]
[row end]


## Lists
- This
- is
- a
- list

* This list

* uses asterisks

* but spaced out a bit

1. This list  (not supported)
2. Is numbered
3. Indeed

* Here is a nested list
    * This is nested further
        1. A nested numbered list
        2. Another list item
        3. One more for good measure
    * Here is the continuation

## Horizontal Rule

Before

----------

After

## Checklist  (not supported)

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

## Blockquote

> You miss 100% of the shots you don't take.
>
> -Wayne Gretzky

## URLs

### Autolinking (not supported)
http://example.com

### Syntax
[Github](http://github.com)

## Font Awesome
Regular size:
@fa-github

Wrapped in header
# @fa-coffee
## @fa-diamond
### @fa-desktop
#### @fa-flask
##### @fa-inbox
###### @fa-mobile

## Code

This is a plain code block:

```
function test() {
  console.log("notice the blank line before this function?");
}
```

This code block has Ruby syntax highlighting:

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

And this one has Javascript:

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

## Tables (not supported)
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Name | Description          |
| ------------- | ----------- |
| Help      | Display the help window.|
| Close     | Closes a window     |

| Name | Description          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

## Emoji (not supported)

:smiley:
:sunglasses:

## XSS Injection (not allowed)

Filtered out or encoded:

<script>alert('bad')</script>
%fe%22
%fd%22
%cd%22
%c1%22
%c0%a2
%80%22
%22

In a image:
![Injection of Src](&#x6A&#x61&#x76&#x61&#x73&#x63&#x72&#x69&#x70&#x74&#x3A&#x61&#x6C&#x65&#x72&#x74&#x28&#x27&#x58&#x53&#x53&#x27&#x29)

UTF-7 injection:
+ADw-SCRIPT+AD4-alert('XSS');+ADw-/SCRIPT+AD4-
