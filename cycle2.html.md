---
layout: default
title: Cycle Slideshows
---

## Cycle 2

Most of these demos can be copy pasted into the site. They will work because Cycle2 is already active on the site.

[http://jquery.malsup.com/cycle2/demo/](http://jquery.malsup.com/cycle2/demo/)

Configure slideshows via HTML data-attributes using the [Cycle API](http://jquery.malsup.com/cycle2/api/)

Example:

	<div class="cycle-slideshow" data-cycle-slides="> a">
		<div class="cycle-pager"></div>
		<a href="#this"><img src="http://placekitten.com/780/280"></a>
		<a href="#that"><img src="http://placebear.com/780/280"></a>
		<a href="#other"><img src="http://placekitten.com/g/780/280"></a>
		<a href="#more"><img src="http://placebear.com/g/780/280"></a>
	</div>

<div class="cycle-slideshow" data-cycle-slides="> a">
<!-- 	<div class="cycle-pager"></div> -->
	<a href="#this"><img src="http://placekitten.com/780/280"></a>
	<a href="#that"><img src="http://placebear.com/780/280"></a>
	<a href="#other"><img src="http://placekitten.com/g/780/280"></a>
	<a href="#more"><img src="http://placebear.com/g/780/280"></a>
</div>

## Pasted example

<div class="cycle-slideshow" 
    data-cycle-fx=scrollHorz
    data-cycle-timeout=2000
    data-cycle-caption="#alt-caption"
    data-cycle-caption-template="{{alt}}"
    >
    <img src="http://malsup.github.io/images/p1.jpg" alt="Spring" >
    <img src="http://malsup.github.io/images/p2.jpg" alt="Redwoods" >
    <img src="http://malsup.github.io/images/p3.jpg" alt="Angle Island" >
    <img src="http://malsup.github.io/images/p4.jpg" alt="Raquette Lake" >
</div>
<!-- empty element for caption -->
<div id="alt-caption" class="center"></div>
