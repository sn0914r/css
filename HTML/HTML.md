### HTML - `HyperText Markup language`
Here:
1. `HyperText`: it means connecting the documents in the web using the `hyperlinks` to navigate to different sections in the same page or to navigate to different pages in the web.

2. `MarkUp`: it represents the `tags` like `<h1>`, `<h2>`, `<p>` etc used to structure content.

3. `language`: represents a language used for structuring the content of web pages.

So, HTML is a language used to structure the content on the webpage and navigate to different sections in the same webpage or to other webpages using the `hyperlinks`.

### HTML Element structure
```HTML
<a href="https://github.com/sn0914r"> hello world </P>
```
Here:
1. `<a>`: is called a`tag`
2. `hello world` is called `content`
3. `href`: is called `attribute`
4. together `<a href="https://github.com/sn0914r"> hello world </P>` is called an `element`.

### types of tags in HTML
#### `container tags` : 
1. These are the tags that has opening tag (`<p>`) and closing (`</p>`) tag.
2. This tags allos us to write some content between them.
3. `<div>`, `<p>`, `<h1> to <h6>` are some `container tags`. 

#### `self-closing tags` or `void tags`
1. These tags doesn't have any closing tags.
2. They don't allow us to write content.
3. `<img>`, `<br>`, `<hr>`, `<input>` are some `self-closing tags`

### attributes
1. The attributes are used to provide extra information to an HTML Element.
2. The attributes are written in the opening tag of an element like `<a href ="github.com">github</a>`
3. The syntax is :
```HTML
<element attribute="value">Content</element>
```
`Example`:
Like if we have an `<img>` tag:
```HTML
<img src="./assets/randomImage.jpg" alt="this is an image" width="400" height="300" >
```
Here :
1. `<img>` is a tag used to display an image.
2. `src`, `alt`, `width`, `height` are attributes, we are providing the extra info like:
    1. `the source of the image` in `src` attribute.
    2. `what to display if image fails to load` in `alt` attribute.
    3. `what width it should be` in `width` attribute.
    4. `what height it should be in` in `heigth` attribute.

### comments in html
1. `comments` are not rendered on the webpage.
2. They are used to write the `documentation` about the code or `temporarily block a piece of code`.
3. The syntax is:
```HTML
<!-- this is comment in single line -->

<!--
this is comment in
multiple lines 
  -->
```

### More about HTML
1. HTML is `case-insensitive` language i.e we can write tags either in capital letters or smaller letters

2. HTML supports `nesting` an element inside another element.
```HTML
<div>
    <p>nested element</p>
</div>
```