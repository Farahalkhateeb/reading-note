# **What is CSS? **

CSS stands for Cascading Style Sheets with an emphasis placed on “Style.” While HTML is used to structure a web document (defining things like headlines and paragraphs, and allowing you to embed images, video, and other media), CSS comes through and specifies your document’s style—page layouts, colors, and fonts are all determined with CSS. Think of HTML as the foundation (every house has one), and CSS as the aesthetic choices (there’s a big difference between a Victorian mansion and a mid-century modern home).
# **External, Internal, or Inline CSS?**
You might be wondering how this CSS code is actually applied to HTML content, though. Much like HTML, CSS is written in simple, plain text through a text editor or word processor on your computer, and there are three main ways to add that CSS code to your HTML pages. CSS code (or Style Sheets) can be external, internal, or inline. External style sheets are saved as .css files and can be used to determine the appearance of an entire website through one file (rather than adding individual instances of CSS code to every HTML element you want to adjust). In order to use an external style sheet, your .html files need to include a header section that links to the external style sheet and looks something like this:

<head>
<link rel=”stylesheet”  type=”text/css”  href=mysitestyle.css”>
</head>
This will link the .html file to your external style sheet (in this case, mysitestyle.css), and all of the CSS instructions in that file will then apply to your linked .html pages.

Internal style sheets are CSS instructions written directly into the header of a specific .html page. (This is especially useful if you have a single page on a site that has a unique look.) An internal style sheet looks something like this. . .

<head>
<style>
Body  {  background-color:thistle;  }
P  {  font-size:20px;  color:mediumblue;  }
</style>
</head>
. . . a thistle background color and paragraphs with 20 point, medium blue font will now be applied to this single .html page.

Finally, inline styles are snippets of CSS written directly into HTML code, and applicable only to a single coding instance. For example:

<h1  style=”font-size:40px;color:violet;”>Check out this headline!</h1>
would cause one specific headline on a single .html page to appear in violet, 40 point font.

Generally speaking, external style sheets are the most efficient method for implementing CSS on a website (it’s easier to keep track of and implement a site’s style from a dedicated CSS file), while internal style sheets and inline style can be used on a case by case basis when individual style changes need to be made.

So if HTML is the foundation, frames, walls, and girders supporting your website, consider CSS the paint color, window styles, and landscaping that comes on afterward. You can’t get anywhere without putting that foundation up first, but—once you do—you’ll want to follow up with some style, and CSS is the ticket to unleashing your inner decorator.