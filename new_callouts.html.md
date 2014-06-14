---
layout: default
title: 'New Callouts'
---

# 'New' Link Callouts

Modify this file to add more callouts

[https://github.com/Hyprtxt/standish/blob/master/scripts/hacks.js](https://github.com/Hyprtxt/standish/blob/master/scripts/hacks.js)

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
