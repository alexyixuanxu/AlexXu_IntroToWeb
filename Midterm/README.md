# Alex Yixuan Xu
[Midterm proposal is posted on this repo]

http://sites.bxmc.poly.edu/~yixuanxu/TheUnknownGameBlog/Home.html [Midterm Website hosted live]

I started coding the website by first doing an html markup for each page.
I put placeholder links to images, texts and notes for future code.
Also at this point, I try to link all pages together.

Then I started to program the CSS for a common feature among all pages, the top navigation.
Using text-align: center I tried to center those elements.

I started to work on the css and interactivity of the navigation. 
To make a hovering effect, so that the link become colored and underlined:
nav ul li a{
	color: white;
	transition: all 0.5s;
}
nav ul li a:hover{
	color: rgb(184,1,65);
}
nav ul li a.Pressed{
	color: rgb(184,1,65);
	text-decoration: underline;
}

I used similar methods to transition throughout the website, such as article links.
I used css filter to add interactivity to images, such as:
main div img{
	filter: grayscale(100%);
	transition: all 0.5s;
}
main div img:hover{
	filter: grayscale(0);
}

For the recommendation page, I wanted to insert a tab before the paragraphs. But it seems that there is no direct way to insert a tab element, so I searched to discover that some whitespace characters can be inserted in text, such as &nbsp;, &thinsp;, &ensp;,and &emsp;.

The most challenging part of this is the homepage slideshow.
To create it, I looked at the tutorials on W3Schools, and adopt their code to my website.
Something I paid attention to:
-The creation of buttons:
<a class="PrevButtom" onclick="plusSlides(-1)">&#10094;</a>
<a class="NextButtom" onclick="plusSlides(1)">&#10095;</a>
-Their use of the <span> tag to group inline elements
-The creation of indicator dot is to have an element that has a background color:
.Dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 5px 2px;
  background-color: lightgrey;
  border-radius: 50%;
  display: inline-block;
}

Still I don't fully understand the javascript used in the image slideshow, such as the "active" part.
The flexibility of the website is also a problem. When I changed the font or make slight changes to margin, it would mess up the whole layout. I also wanted to know an easier way to vertically align elements. Manually setting padding doesn't seem to be flexible enough.
Though the use of filter is really intereting, it doesn't necessarily work on all browsers.
If I have more time and more tools, I would try to integrate my own p5.js sketches into the website to make it more fun, more animation for the slideshow, design it better to make it more visually appealing.