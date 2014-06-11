---
layout: default
title: 'New Callouts'
---

# 'New' Link Callouts

This is the commit that added the buttons:

https://bitbucket.org/reapmarketing/new-standish-template/commits/9f043b0333356946623e717c1835e26aeaa17397

## Adding the element with JavaScript

The Important Bit:

```JavaScript
   $("a.cat:contains(Supplies)").append('<span><i class="icon icon-star"></i> New</span>');
   $("a:contains(Break Room)").append('<span><i class="icon icon-star"></i> New</span>');
```

Each line adds a "New" element.
These target the links `a` by text content. Notice how `Supplies` uses the `.cat` class to speficiy the sidebar.

## Styles

Here are the styles, you shouldn't need to change these.

```CSS
	.navigation ul ul a span,
	.cat span {
		background: #dfe133;
		padding: 2px 5px;
		border-radius: 2px;
		margin-left: 5px;
		color: #696969;
	}
	.navigation ul ul a span {
		position: absolute;
		padding: 2px 2px 0px 2px;
		top: 2px;
	}
```
