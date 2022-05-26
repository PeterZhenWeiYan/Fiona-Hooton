The theme of this website is to introduce Fiona Hoonton. The website has three pages: Home, About, and Contact. The responsive development of the website is realized by using the media query `@media` in CSS3, which is compatible with responsive desktops, tablets and mobile devices.

This website is a personal introduction website. Compared with most current websites of the same type, there are relatively few page contents, and the page design and layout are not perfect, which will cause the entire website to fail to attract users better.

## Technical achievements

Using html5+css3 to complete the production of the entire website

The production level of the website is about medium. Before starting to write the code, I checked some precautions for making a website, such as css style reset and extraction of the same style, which can improve the level of the code, and there is a reason for code reading and maintenance.

### css initialization

CSS initialization refers to resetting the browser's styles. Different browsers may have different default styles. So maybe the first thing in development is how to unify them. If the CSS is not initialized, there will often be page differences between browsers. Every time we develop a new website or a new web page, the attributes of the CSS style are used to make the CSS or HTML tags we will use more convenient and accurate, which makes it more convenient and concise when we develop web content, reduces the amount of CSS code, and saves web page download time. The css initialization code is as follows:

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html,
body {
    font-family: 'Courier New', Courier, monospace;
    font-size: 20px;
    color: #000;
}

ul,
li {
    list-style: none;
}

a {
    color: #000;
    text-decoration: none;
}

img {
    max-width: 100%;
}

/* Custom style */
.fl {
    float: left;
}

.fr {
    float: right;
}

.cl::after {
    content: "";
    clear: both;
    display: block;
    visibility: hidden;
}


.h20 {
    margin-bottom: 20px;
}
.container {
    width: 1200px;
    margin: 0 auto;
}
```

### css selector

Css selectors used in web pages mainly include wildcard selectors, tag selectors, class selectors, descendant selectors, structural pseudo-class selectors, and union selectors.

## problems at hand

Regarding the multi-terminal compatibility effect of the responsive website, when using css @media technology to make it, it is found that the style written does not take effect. After consulting the data, I know that a line of code needs to be added to the <head> header:

```css
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## Project reflection

Through the production of this website project, I have learned the correct way to make a responsive website. First, we must determine the theme of the website, and then start from which sections to create around the theme, that is, the columns of the website, and determine the style, tone and main body of the website. Width, font size, etc., and the compatibility of each browser should be guaranteed when the production is completed. The disadvantage is that the overall function of the website is relatively simple. A complete personal website needs to be introduced from multiple aspects, such as hobbies, works display and so on.

At the same time, in the project development, for the production of responsive website, it is necessary to consider the compatibility of multi-terminal response, that is, the webpage can be displayed perfectly under different screen widths. Different styles are set for the screen size; when you reset the size of the browser, the page will also re-render the page according to the width and height of the browser;

