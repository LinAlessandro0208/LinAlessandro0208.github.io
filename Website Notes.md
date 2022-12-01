# HTML 
# Shortcut
If you write ! and then hit tab it will automatically write 
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
If you write `tag*3` it shows 
```html
<tag> </tag>
<tag> </tag>
<tag> </tag>
```
If you write tag1>tag2*3 it shows
```html
<tag1>
    <tag2> </tag2>
    <tag2> </tag2>
    <tag2> </tag2>
<tag1>    

```


# Heading
```html
<h1> Heading level 1 </h1>
````

## Heading level 2
```html
<h2> Heading level 2 </h2>
````

### Heading level 3
```html
<h3> Heading level 3 </h3>
````

#### Heading level 4
```html
<h4> Heading level 4 </h4>
````

##### Heading level 5
```html
<h5> Heading level 5 </h5>
````

###### Heading level 6
```html
<h6> Heading level 6 </h6>
````


# Paragraphs
This is a paragraph
```html
<p> This is a paragraph </p>
```


# `<div>` Tag
The `<div>` tag is a block element.
```html
<div> a </div>
```

# Navigation
Navigation bar




# Line Breaks
To create a line break or new line.

This is the frist line 

This is the second line
```html
<p> This is the first line. <br> 
This is the second line.</p>
```


# Bold, Italics
**Bold**, _Italics_
```html
<strong>Bold</strong>
<em>Italics</em>
```

# Button
```html
<button>Button</button>
```



# List
Unordered list
- Item 1
- Item 2
- Item 3
- Item 4
```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
</ul>
```
Ordered list
1. Item 1
2. Item 2
3. Item 3
4. Item 4
```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
</ol>
```
The first item is defined as
```html
li:first-child{

}
```


# Header
The `<header>` element defines a header.
```html
<header> Header </header>
```

# Section
The `<section>` tag defines a section.
```html
<section> Section </section>
```

# Footer 
The `<footer>` tag defines a footer.
```html
<footer> Footer </footer>
```


# Link
Hyperlink reference
[link name](doc.html)
```html
<a href:"doc.html"> link name </a>
```
Hyperlink reference with folders
```html
<a href:"folder name/doc.html"> link name </a>
```
Hyperlink reference with upper level (folder before)
```html
<a href:"../doc.html"> link name </a>
```
You can link a stylesheet with
```html
<link rel="stylesheet" hre="folder name.css"> 
```


# Figure
To insert a figure
```html
<figure>
    <img src="file name.jpg" alt="">
    <figcaption> Caption </figcaption>
</figure>
```












# CSS
# Style
You can define the properties of selectors, by giving values, using `<style> </style>`.
```html
 <style>
    h1 {
        background: white;
        color: red;
    }
    h2 {
        background: white;
        color: rgb(93, 93, 93);
        opacity: 0.5;
    }
    body {
        background: rgb(58, 58, 58);
        color: black;
        font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
        text-align: left; <!-- left or right>
    }
    header {
        background: white;
        color: black;
        margin: 20px;
        padding: 29p x
    }
    section {
        background: white;
        color: black;
    }
    div {
        background: white;
        color: black;
        display: block;                 
    }

    log {
        background-image: url("file name.png");
        background-size: 300px; 
        background-repeat: no-repeat; <!-- the image will repeat-->
        background-position: center;
        position: relative;
        top: 0;
    }


    footer {
        background: white;
        color: black;
        font-size: 12px;
        text-align: center;
        padding: 20px 20px;
    }

    figure{
        border: 1px solid white;
        margin:auto;
        border-radius: 50%          /* border circle 
                                    with radius */
        box-shadow: black 0 0 10px;
        width: 200px;
        text-transform: lowercase; /* upper case */
    }
</style>
In CSS do not put <style></style>
```
## Selectors
Only selectors which is inside of another selectors

`footer` which are inside `div`
```html
    div footer{

    }
```
two selectors with same properties and values
```html
    div, footer{

    }
```
You can add classes to selectors
```html
<selector class="class1">
<selector class="class1 class2">
```


To remove the edge
``` html
    margin: 0;
    padding: 0;
```

## Margin
Margin applies `20px` to all sides
```html
    margin: 20px;
```    
Margin applies `20px` to top and bottom and `40px` to left and right
```html
    margin: 20px 40px;
```    
Margin applies `20px`top, `40px` right, `10px` bottom and `50px` left
```html
    margin: 20px 40px 10px 50px ;
```  
Margin applies only on one direction
```html
    margin-top: `20px`
    margin-right: `40px`
    margin-bottom: `10px`
    margin-right: `50px`
```

## Padding 
Padding adds that space inside the box and it works exactly like margin does.


## Display
Displays an element as a block element
```html
    display: block
```
Displays an element as an inline element. Any height and width properties will have no effect
```html 
    display: inline
```
Displays an element as an inline-level block container. The element is formatted as an inline element, but you can apply height and width values	
```html
    display: inline-block
    height: 80px;
    width: 300px;
```
Displays an element as a block-level flex container
```html
    display: flex
```
Flex direction
```html
    flex-direction= row;
    flex-direction= column;
```    

Remove bulletpoint
```html 
    list-style-type: none;
```
Hyperlink not underlined
```htlm
a:active{
    text-decoration: none;
}
````
Hyperlink when you hover the underline disappear
```html
    a:hover{
        text-decoration: none;
    }
```
Hyperlink when you hover the underline appear
```html
    a:hover{
        text-decoration: underline;
    }
```




# Different Device use
Too extend
```html 
@media screen and (min-width: 400px){
    .features {
        background: white;

    }
}

@media screen and (max-width: 800px){
    .features {
        background: white;

    }
}

```