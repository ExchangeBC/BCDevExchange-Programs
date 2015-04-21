Markdown test
=============

This is a test for Markdown capabilities.

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

This sentence has some *emphasis*, and it also **embiggens** the smallest man.

~~Mistaken text.~~

Here is some cool `monospaced` text.

This is an image!
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

# Lists
- This
- is
- a
- list

* This list

* uses asterisks

* but spaced out a bit

1. This list
2. Is numbered
3. Indeed

* Here is a nested list
    * This is nested further
        1. A nested numbered list
        2. Another list item
        3. One more for good measure
    * Here is the continuation

## Checklist

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

# Blockquote

> You miss 100% of the shots you don't take.
>
> -Wayne Gretzky

# URLs

## Autolinking
http://example.com

## Syntax
[Github](http://github.com)

# Code

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

# Tables
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

# Emoji

:smiley:
:sunglasses:

# Injection
<script>alert('bad')</script>
