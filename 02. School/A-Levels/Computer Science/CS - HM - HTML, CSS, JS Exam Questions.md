---
title: CS - HM - HTML, CSS, JS Exam Questions
category: A-Level
subject: Computer Science
topic: Exam Practice
date: 2025-03-04
tags: [A-Level, Web-Technologies, CS, Computer-Science]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on practising HTML and CSS Exam Questions
# Q1
One advantage of storing CSS in an external file over embedding it within HTML is that it prevents repetition of styling and allows for modularity as you can set a style for a whole tag or class instead of having to style each element in the HTML file.
## *Covered*
More organised
Loads faster for user
Inline would needed to changed for **every** line but in an external CSS file, change it once and its changed everywhere
# Q2
## Part (a) & Part (b)
```html
<html>
<head>
<title>My Stamp Collection - European Stamps</title>
</head>
<body>
<h1 style="font-family:Arial; color: darkGreen"> United Kingdom</h1>
<p>These are my stamps from the uk.</p>
<img src="UKstamps.jpg"/>
<a href="http://ukstampcollectorsguild.co.uk">Find out more about UK stamps as a link to the UK Stamp Collectors Guild website which has the URL:</a>
```
## Part (c)
### Part (i)
One disadvantage to the owner of styling attributes in tags instead of a linked CSS file is that it lacks modularity and involves a lot of code repetition
### Part (ii)
One disadvantage for the site's visitors is that the site could load slower to access as the information is reloaded every page
## Part (d)
```css
body {
	background-color: lightGreen
}
```
# Q3
```html
<h1>Reasons to Choose Us</h2>
Come play <em>Laser Tag</em> with us for:
<ul>
	<li>State fo the art equipment</li>
	<li>Friendly staff</li>
	<li>Match recordings available to purchase</li>
	<li>Buy two games get one free</li>
```
# Q4
## Part (a)
```css
# warning {
font-family: "monospace"
color: "red"
}
```
## Part (b)
`<input type="text" name="username">`
This line *provides a text field and* accepts a text input from the user and relates the input to username
# Q5
One measure that can be taken to ensure the website is accessible is the use of a colour contrast which allows for text to be easily read on the webpage for people with vision impairments. Another would be using appropriate headers which make different sections
## *REDO*
AO1 Knowledge - 4 -> Definition
	Application - 2 -> Context
	Evaluation - 3
AO1 Points: Define what would make a website accessible and why is it important to make it accessible
	Websites that are designed to allow people with disabilities to comfortably use them and navigate the website.
	Different sized devices (touchscreen or mouse)
	Define technical measure
AO2 Points: Talk about what device is being used, disabilities, screen-readers, different languages
	Translation: Auto Translator (but AO3, can be inaccurate ) or make a website specifically for that language
	Bigger items, elements, text, etc...
	How to implement it (alt text, text contrast, text sizing, alternate languages, headings, colourblind-friendly)
AO3 Points: What are some drawbacks and benefits (more accessible brings more traffic, accessibility requires more code and more code can lead to more bugs)

## Timed Answer
Accessibility is when a website is designed to allow people with disabilities or who speak another language to be able to comfortably use and navigate a website. Having an accessible website is important as it ensures that everyone is able to use the website with no or little difficulty. This can also be applied to people using different devices with different screen sizes or different pointing devices such as a mouse, touchpad or touchscreen so they too can use the website comfortably and effortlessly.
	One way to implement accessibility for users who speak other languages would be to implement a translation feature whether through an auto translator or designing a version of the website specifically for a certain language.
	Another way to implement accessibility would be to use appropriate headings and use bigger items, icons, elements and text so that people with vision impairments or disabilities are able to adequately view the page.
In regards to the translation feature, using an auto translator has the benefit of being cheaper and easier to implement but at the cost of potentially inaccurate translations which would negatively impact the user's experience. If a website is made to be accessible, it has the potential to gain more user traffic as it is more suitable and accommodating for more people which is beneficial when running and hosting a website. However, with implementing accessibility, a settings feature would also need to be implemented to allow users to pick and choose what accessibility features they want and implementing accessibility involves more code which means there is a greater chance of bugs.

# Q6
A HTML id attribute can only be used for one element but a HTML class element can be used for multiple elements
# Related Questions