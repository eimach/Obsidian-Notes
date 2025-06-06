---
title: CS - HM - HTML & CSS
category: A-Level
subject: Computer Science
topic: Web Technologies
date: 2025-02-20
tags: [A-Level, Computer-Science, Web-Technologies, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - HM - Web Technologies]]
Tags: #CS 

# Definitions
- HTML: Hyper-Text Markup Language
- CSS: Cascading Style Sheets
- JS: JavaScript


> [!NOTE] What do they do?
> HTML acts as the skeleton of the website, CSS works as the skin/looks of the website, JavaScript acts as the brain of the website.

# Syntax
## HTML
``` HTML
<!DOCTYPE html> - %% declaration --> this shows that the document is a HTML5 document %%
<main></main> - %% indicates main content of website for SEO reasons %%
<body></body> - %% contains everything that should be rendered on the page %%
<head></head> - %% used to contain metadata. e.g. title, links to stylesheet and scripts %%
<head>
    <link rel="stylesheet" href="styles.css">
</head> - %% links to a styles.css file for website styling %%
<h1></h1> %% h1 -> h6 %%
<p></p> - %% paragraph %%
<img></img>
	<img src="image.jpg" alt="example alt text"> </img> %% links to an image and adds alt text in case of image not loading %%
<div></div> - %% dividers %%
<a></a> - <a href="link"> </a> - %% anchor, can use for hyperlinks %%
<section></section> - %% seperates elements into section %%
<ul></ul> - %% unordered list %%
<ol></ol> - %% ordered list %%
<li></li> - %% creates list items in unordered/ordered lists %%
<figure></figure> - %% lets you associate an image with a caption %%
<figcaption></figcaption> - %% adds a caption to a figure element %%
<em></em> - %% emphasises (italics) text %%
<hr> - %% adds a divider line %%
<strong></strong> - %% bold text %%
<form></form> - %% used to gather information from users %%
	<form action="link"></form> - %% points to where form data should be saved %%
	<input> - %% allows ways for data to be collected - DOES NOT REQUIRE CLOSING TAG %%
	<input type="text"> - %% lets user input text %%
	<input type="checkbox"> - %% lets user tick a checkbox %% 
	<input type="text" name="example"> - %% something %%
	<input type="text" placeholder="example"> - %% gives user an idea of what kind of information to input %%
	<input type="text" name="example" placeholder="example" required> - %% ensures that user can't submit form without entering certain information %%
	<input type="radio"> Radio - %% used when you only want one answer out of multiple options - VOID ELEMENT %%
	<button>Submit<button> - %% creates clickable button -- Inline Element %%
	<button type="submit">Submit<button>
<fieldset>
	<legend> text </legend> - %% acts as a caption for fieldset %%
		  </fieldset> - %% nests group related inputs and labels together in a web from - is a block level element %%	
```
## CSS
``` css
element {
 property: value;
} - %% allows you add style to an element when in a <style> element %%
#id { - %% id selector: assigns a style to an element with that id %%
 property: value;
 width: 300px - %% sets width of an element to a specified value %%
 width : 80% - %% makes width a % of its parent element %%
}
.class { - %% class selector: same as id selector but for classes %%
}
<element class="class name"> - %% sets style to that of the class %%
<article></article> - %% elements which typically contain multiple elements with related information %%
{
display: inline-block - %% makes whatever element has this styling to be displayed inline %%
}
```