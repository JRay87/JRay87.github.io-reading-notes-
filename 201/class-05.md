# Reading 5

## HTML Chapter 5 - ***Images***

<img src="images201/robbie-noble-JGcaxNi2fQ8-unsplash.jpg" alt="Baseball Hat" title="Mets Hat by Robbie Noble"/>

Images can be used to relay information in a visualy appealing way and can have a major impact on the appeal of your site. One example of an image added to your site through is the following code:

`<img src="images201/robbie-noble-JGcaxNi2fQ8-unsplash.jpg" alt="Baseball Hat" title="Mets Hat"/>`

You can then use placement in HTML to change to how the image interacts with other content within your page. This can be done in HTML as well:

- Before p tag - text starts under the image
- Inside the opening p tag - text starts inline with the bottom of the image
- Inside the text - the text will display on the same level as the image

Following CSS rules you can also manipulate the image around the page. Changing size, placement, opacity etc.,

If you are using images remember, `.jpgs` for vivid images, `.gifs` (pronounced 'gifs') for simple images. (Please use animated gifs sparingly)

New in HTML5 is `figure` and `figcaption` These are used to display images with text as a caption under the image.

## HTML Chapter 11 - ***Color***

With CSS rules we can change many different features besides just putting color on the screen (`background-color:`) and text color (`color:`).

To really understand how we can effect the colors on the screen, we should first understand how the color value is expressed in CSS. Color can be expressed in RGB value, hex codes, or with the name (if the name has been pre-defined). Hovering over the color square also gives the developer access to a color square with sliders etc., to make any custom color combination.

From there they can also change the hue, saturation, or brightness.

Developers should remember that high contrast text is best for most text options because it makes the text easier to read. This changes however as the amount of text grows. Too much high contrast text leads to eye strain for the user, so pay close attention.

CSS3 gives the developer to some new color rules. These other color settings include the Opacity (`opacity:`) which makes the color more see through as the opacity decreases(?).

## HTML Chapter 12 - ***Text***

Text and Typeface are the primary modes of relaying messages through your websites. Obviously this makes it (the content) the most important aspect of your site. Chapter 5 begins with a discussion on different text aspects and how they impact the characters on the screen. From weight and style to stretch they will all have a different effect on the typeface (font - but with the previously mentioned info).

- `font-family` - designate the specific typeface you want
- `font-size` - the display size of the typeface (can be in pixels, percentage or 'ems'<-the width of the letter m 1 em)
- `font-face` - displays typefaces that aren't installed on users browser. (requires licensing)
- `font-weight` - creates **bold** text
- `font-style` - displays the text with italics or obliques
- `text-transform` - displays font in uppercase, lowercase, or capitalization of first letter
- `text-decoration` - underline, overline, linethrough, blink (don't do it Johnny)
- `line-height` - raises or lowers the entire line of text (similar-ish to subscripting)
- `letter-spacing`/`word-spacing` - expands the white space between letters
- `text-align` - similar to justifying text on a word document
- `vertical-align` - aligns where the text is displayed in connection with inline elements
- `text-indent` - indents the first line of text within an element
- `text-shadow` - Creates a drop shadow of the text
- `:first-letter`, `:first-line` - used to modify these specific portions of the text
- `:link`, `:visited` - sets the styling of the links prior to and after click
- `:hover`, `:active`, `:focus` - hover can be used to change display when mouse is on a link but hasn't clicked. active is how it reacts when clicking is in progress. focus is tells the browser to give focus to where the mouse is located (?)

There are tricks to target very specific elements. They are called attribute selectors and can be used to make CSS rules for elements within multiple parent elements without having to write code for each instance.

## JPEG vs PNG vs GIF by *Rahul Nanwani*

### [Link to the article](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

JPEGS:
- Best for natural scenes or vibrant photos. 
- It is a '*lossy compression specification*' and achieves 1:10 compression ratio.
- Don't support transparency.
- Can support about 16mil different colors
- Doesn't support animations

PNG:
- Best for images needing transparency or images with text 
- '*retain higher quality...than JPEG...also occupy(s) more space on the disk*' 
- A good option for images with text, logos etc., 
- Allow transparency in two ways. Partial '*makes the edges blend smoothly into the background*' while index makes a single color transparent.
- PNG8 supports 256 colors, PNG24 - 16mil
- Doesn't support animations


Gifs:
- Images with animation
- Generaly '*unsuitable for images with transparent backgrounds.*'
- Supports 256 colors

## What I want to know more about

- Opacity values impact on the element
- What is focus?

<img src="https://media.giphy.com/media/TGWklzt8RZvjV16O8n/giphy.gif" alt="Silicon Valley gif" title="Silicon Valley gif"/>

gif found on [giphy.com](giphy.com)