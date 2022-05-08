# ***Intro to HTML, and Design basics*** 

Congrats on making it to 201! Now that you've had the time to digest the information you learned in 102 it is time to dive right into the material for this course. In this lesson we read from Jon Duckett's book, *HTML & CSS* as well as a chapter from his other book *JavaScript & JQuery*. Let's start off with what we read in his book on HTML. 

## *HTML&CSS* **Intro**
The introductory chapter had some basic information on how the internet works and how they interact with the network as well as the browers used (IE,Chrome,Firefox) to display the HTML document. This chapter was short but a great intro to web design for people with minimal knowledge and/or experience. 

## *HTML&CSS* **Chapter 1 - Structure**
We continued on to chapter 1 - titled *Structure*. This chapter was about what structure is and how it is useful for, not only webdesigners, but anyone who is trying to figure out how to relay information to people with most enjoyable and efficient experience possible. Structure, in this context, is used to describe the way in which you style your HTML document and the elements written within. (As a quick reminder to readers, websites are "merely" a text document written with HTML in such a way that an internet browser such as Chrome or Firefox can translate it to display the webpage to a user. Also, an element is the code written to include everything within the opening and closing tag.)

`<p lang="en-us">Let's Go <strong>METS!</strong></p>`

In the above example the HTML structure is translated by the browser to be displayed as:

><p lang="en-us">Let's Go <strong>METS!</strong></p>

As you can see from the code above tags that are opened must be closed and the opening tag is where you can put the tag attributes. I notified the browser that there was going to be text in the `<p>` tag, where I also stated the text would be in US English. Then I let the browser know that I wanted the text 'METS!' to be emphasized with bold.

This is just a taste of how a text document impacts the information seen on your browser. As I continued with the reading I learned more about the structuring and how it changes what is displayed in the browser.

## *HTML&CSS* **Chapter 8 - Extra Markup**

This chapter focused on more of the elements, tags, attributes, etc., and how they impact what is displayed by the browser. One of the most important of which would be the Doctype or ` <!DOCTYPE html>` (as written in HTML5). This is one of the most important not only because it is found at the top of the text file, but because it tells the browser what type of document they are looking at. Without the Doctype to tell the browser what it is written below the browser wouldn't know how to translate the language into a workable site. Another important Markups you can use within an HTML document will never be displayed to the user (and that's the purpose). 

When programming a site for users the developer should find ways for others to be able to read the code. One such technique is to make *comments* within the document. This can describe what a section of code is accomplishing or just simple housekeeping information for future developers working on the code. 

>`<!-- Text in here will not be displayed -->` <-Comment Code

If you're looking to specify an element for formatting, separately than the general element(p,div,span,article, etc.,), you can put an id on the tag by adding (using a p tag for example) ` <p id="NAME">`. Alternately if you're wanting to put classes on similar elements you can add `<div class="NAME">`. These concepts will become more important as we get into CSS, but for now it can be useful for your code housekeeping.

One final item from the chapter I'd like to bring up is the meta element. This needs to be kept in the `<head>` section of your code as it stores information for your site. The browser does not display it, but the information is important. 

    <head>

        <meta name="(Website's name)"
            description="(Quick site description)"
            keywords="(words users might search for, no SEO impact)"
            robots="('noindex'- not searchable,'novalue'- searchable )"
            author="(Website's author)"
            pragma="(This will keep the browser from storing the website for fast retrieval)"
            expires="(This allows the browser to store the page for a set time before deleting cache)">
    </head>

<!-- I'm not sure how to talk about block/inline and the div/span connection without this section going long. But in summation 'Block' groups down , 'Inline' groups right. 'Div' is a block grouping, 'Span' Inline grouping.  -->


## *HTML&CSS* **Chapter 17 - HTML5 Layout**

This chapter started off with a breakdown of the changes made from the older HTML formats and *HTML5*. Quick note - HTML5 has not been fully released but is the newest edition being used by the industry. The book states that developers can: 

>"take advantage of the new features of the language as long as you endevour to ensure that users with older browsers will be able to view your pages (even though some of the features will not be visible to them)." ~pg 180

I'm not sure what this means. For example, one of the features of HTML5 is less tags needing a closing tag to operate properly; if I don't use a closing tag, would older browsers not display the webpage correctly? And if that's the case, how accepting of HTML5 are browsers, *really*?
    
    - This was answered later in the book. To properly display HTML5 in older browsers there are lines of code that need to be added to the CSS and HTML file.

   <strong>CSS</strong>

    `header, section, footer, aside, nav, article, figure, figcaption {
       display: block;}`

<strong>HTML</strong>

    `<!--[if lt IE 9]>
    
    <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    
    <![endif]>`


(Back on track now) One noticeable change in HTML5 (for veteran coders) is that the HTML has lessened its reliance on the `<div>` element. To better designate sections of the document, developers will use:

`<nav>` - Holds the navigation code, which contains links to different sections and pages within your website.

`<article>` - This will contain the most important segment of content from your site.

`<aside>` - If inside an article tag the info is related to the article but not super important for the article. If outside an article tag the information relates to the entire webpage.

`<section>` - You can use this multiple times to group like content together (to section it off from the main content), or you can use it to put a break in a long piece of content.

`<hgroup>` - This is used to group the `<h1>`-`<h6>` elements. 

`<figure>` - In HTML5 developers can use the figure tag to contain many different forms of media (image, video, graphs, etc.,)

   - `<figcaption>` - attached to this is the inclusion of the figcaption tag which allows for a text description of the media it is connected to.

`<div>` - The div tag didn't leave us in HTML5 but it is now to be used if the content does not fit in any of the other tags.

It was interesting to see some of the evolution of the syntax as the internet has advanced throughout the years.

## *HTML&CSS* **Chapter 18 - Process and Design**

Over the last few chapters I have noticed the overarching concept of formatting or stylization that can be completed through HTML code. Before even a single line of code is written however, a good developer takes the time to build a profile of the expected users and a layout of the website or app.

Is this site/app for personal or business uses?
- If for personal use you should build a profile on these users that include age range, income, education, etc.,
- If this program is for a business, what's its size? Who's using the program (corporate/mid level/entry level)? etc.,

Then you look closer at your target audience. Why are they coming to your site? What are they trying to accomplish? Are they shopping for digital media or uploading earnings reports? How often are they going to be coming back? These types of questions can help form a profile of who the users are, what they are needing to do, and what information you are needing to get to them to achieve this.

Taking all of this information a coder can then build out a sitemap of what they are needing to accomplish for the user to have the most efficient and enjoyable experience possible. A *sitemap* will spell out what information is needed to relay to the user and will help organize these sections into pages for your website.

The book identifies one technique called *card sorting* (pg 461). This technique has the developer putting the types of information the user would need on individual pieces of paper or flash cards etc., Something physical that you can then group into related segments which can then become an individual page. The physical items and actions can prove helpful in the development process.

From a sitemap the developer should then design a *wireframe*. This is similar (in concept) to a siteframe for an individual page, but the developer will design a shell of what the individual page will look like. You do not put the actual content on the page, but you lay out where it will go. This is all in service of when you sit down to do actual coding. Think of it like storyboarding a movie/tv show. The development team maintains an overview of the final product while being able to work on individual segments.

After all this reading regarding different ways to format your content, you may be asking yourself why does it matter. I feel the author may have been aware the reader would be doing this as he ends chapter 18 with a section on visual design. Visual design helps the developer relay their message/information to the user and in turn help the user achieve their goals. 

This can be done with more outwardly recognizeable things like links easing traversal through the site, putting your most important info near the top (*prioritizing* p465), or putting text over an image relating to your product or service (*visual hierarchy* p465). 

Visual Hierarchy helps readers find their information quicker. Larger text telling the readers of new info (like the headers above designating a new chapter's material) make it easier for you to find which chapter you're looking to learn about. Different colors in the headers also make it easier to know where these breaks are. Same with stylizing the text with bold and italics. It all is done to allow the user to efficiently locate what they are trying to find. 

How sites group their content can have an impact on the users experience as well. The use of *proximity*, *white space*, or *borders*, etc., (p469) can give the user visual representation of the location of information. Content located near eachother is generally expected to be related and through these and other grouping styles can help keep that information flowing smoothly.

Finally the author discusses the principles for navigation design. There are six general rules to remember. Keep your links:

- Concise - quick, easy to read.
- Clear - describes what the user should expect on the linked page.
- Selective - Only take to the main pages. Further links can be there.
- Context - Indicator of users current location.
- Interactive - Links big enough to see and use easily, reacts to user input.
- Consistent - Keep your primary navigation the same style throughout the website.

## *JavaScript* **Intro & Chapter 1a - ABC of Programming**

As a reminder, JavaScript is what makes your website interactable. With JavaScript you can access or modify content (as seen with forms) or you can program visual changes to content like highlighting links, or displaying text descriptions when hovering over a link or image. This can all be completed using Javascript. (Remember that some older browsers do not interact properly with new additions to coding languages. Later on in the reading we will learn about jQuery)

**1a** discussed designing scripts and the proper procedure to formulate your code before sitting down at your computer. 

Mr. Duckett defines a "Script" as
> "a series of instructions that a computer can follow to achieve a goal."(p14)

Scripts are run to complete a task based on the inputs by the user. To complete these tasks, however, the developer needs to write out the program step by step and define the variables for the computers to be able to translate them correctly.

So when we as developers sit down to script code we have to follow some steps (as laid out on  pg 17)
>Define the goal - What are you trying to achieve?

>Design the script - What steps are needed to complete the task?
    
> Use a flowchart to help visualize the steps needed, in order. 

>Code each step 

1b discussed objects & properties, events, and methods.