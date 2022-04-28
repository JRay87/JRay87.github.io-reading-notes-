# ***Cascading Style Sheets*** (Let's get this place looking nice)

## What is CSS

CSS is a coding syntax that is used to tell the browser how to present the documents to the user (A "document" is a text file structured with markup language). These documents are shown to the user on a browser and these are programmed to translate the code into a website. Hopefully one that is easy on the eyes and even easier to use.

CSS can be added to code for an HTML document in any of the following three ways.
	- External - This is considered the best way to handle CSS as you do all of your coding in a seperate tab and then add it to your HTML with one simple code. 

> `(INSERT CODE HERE)`

	- Internal - This style can be found useful if there is one page within your repository needing special formatting seperate from the rest of the files. To complete internal CSS you would simply code all your desired CSS formatting directly onto the top of the HTML, maintaining proper CSS syntax.

> `(INSERT CODE HERE)`

	- Inline - Inline is the most difficult form of CSS because the code is placed directly on the element it is modifying. It can quickly cause issues within your html document and also makes it difficult to traverse the code, making debugging all the more difficult. (Long story short, try to keep this to a minimum.) 

> `(INSERT CODE HERE)`


## So you ready to give it a shot?

For the purposes of this practice we are going to focus on External CSS. First things first, make sure you have your website's wireframe handy (It can really help keep your coding on track). To initiate a CSS file you will simply open the repository for the website you are going to be working on, and create a new file within that folder. Keep the name simple and one word just make sure it ends in ".css". After this file is created, insert the file name into the code above and put the line of code in the top of your `<head></head> brackets. 

Looking at your wireframe (remembering the box method) start from the top and work your way down. What is the header section going to look like? How about the font in the text? Or its placement when near images. All of this can be controlled with just a few of the many CSS changes you can make. The basic format of a CSS code would look as follows. (I'll break down what you're reading afterwards.) 

` header {
	border: 5px, solid orange;
	background-color: blue;
	color: white
     }`

To start, "header" shows the browser that this bit of code is focused on any section labled header within the page. Open bracket (its shift+ the key next to P) tells the browser that the way it is to be displayed is coming up. Border (meaning the border around the header box) is to be 5 pixels thick, solid, and orange. Background-color is going to be filled in with a beautiful shade of blue. Lastly "color" means the color of the text used within that section. So if you were to have an html document with the code...

`<header>
	<p>Let's Go Mets!</p>
</header>` 

...the website would present you with an Amazin' Mets themed banner in the header section of your wireframe. There are so many other ways you can modify the presentation of your site through CSS. Click [here](PUTWEBSITELINKHERE.COM/CSSCHEATSHEET) for a quick list of the various options. Now go have a little fun and mess with your site a little. 

Click [here](README.MD) to go back to the home page.