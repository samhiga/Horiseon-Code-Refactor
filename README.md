# horiseon-code-refactor

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    

## Description 

[Visit the Deployed Site](https://samhiga.github.io/Horiseon-Code-Refactor/)

This webpage provides information on the Horiseon marketing agency. Given the starter code, the task was to make sure the HTML elemants were semantic, that there was a logical structure to the code, that the images were accessible through alt attributes, and that overall everything followed a professional and clean format. The result was a website that still maintained its look and function while code has been properly organized and adjusted. 


## Table of Contents (Optional)

* [Code Refactor Example](#code-refactor-example)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Author Info](#author-info)
* [Credits](#credits)
* [License](#license)


## Code Refactor Example

Using the Github clone this repository into your local machine using Terminal or Gitbash. Navigate to wherever you have cloned the files and use a code editor to view the HTML and CSS files. Using the deployed link, you may also view the site. Using the navigation bar will take you to a section of your choosing on the page.


```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

Converting the above non-semantic div with the class of 'header' to an appropriate [<header> semantic element](https://www.w3schools.com/html/html5_semantic_elements.asp). 

```html
<header>
        <h1>Hori<span class="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>

```

This change require some additional modification to the CSS selector: 

```css
.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}
```

No longer targeting the element on the page with the class of 'header' but instead the css selector targeting the 'header' element 

```css
header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

```

Some alt attributes where added to the images as well to make them more accessible 

```html
<img src="./assets/images/search-engine-optimization.jpg" class="float-left" alt="seo notebook"/>
```

## Usage 

The website is to be used to inquire more information on what Horiseon marketing agency provides its customers while also providing a smooth and functioning user experience that meets accesibility standards. The HTML and CSS files are also meant to be accessible by being easily readble and easy to follow along to give a good understanding of the structure of the website.


## Learning Points 

Through this project, I was able to obtain a lot of new information. TMuch of the information gained was in how to make HTML elements semantic
as well understanding how to make the CSS sheet correspond to this change as well. My ability to pinpoint and identify potential bugs within the 
code has improved as well and generally given me a better understanding of what code does what.


## Author Info

```md
### Sam Higa 


* [LinkedIn](https://www.linkedin.com/in/sam-higa-b887b9209/)
* [Github](https://github.com/samhiga)
```


## Credits

Starter code was acquired from "The Coding Bootcamp" through the urban-octo-telegram repository on Github.
[The Coding Bootcamp Github Page](https://github.com/coding-boot-camp)

Tutor Brandon Rose assited me with understanding HTML and CSS semantic elements.

---


