## tags
### text formatting tags:
1. `<h1>` to `<h6>`: 
    1. these tags are used to define headings or title on a webpage.
    2. all the `<h>` tags are bold by default
    3. `h1` is largest and most important, `h6` is smallest and least important
2. `<p>`:  used to define a paragraph of text
3. `<b>`: for bold text
4. `<i>`: for italic text
5. `<strong>`: for bold + important text
6. `<em>`: for italic + important text
7. `<u>`: for underlined text
8. `br>`: to inserts a line break (`self-closing tag`)
9. `<hr>`: to inserts an horizontal line (`self-closing tag`)

### Grouping
1. `<div>`:
    1. `<div>` is a container elements allows us to next `nest` multiple elemenst into it.
    2. It is very useful when we need to target a group of tags for styling or scripting purposes.
    3. it's a `block level` elemnet i.e it occupies the full width in the webpage.
    ```HTML
    <style> div{ color: red } </style> <!-- applies red color to every element in the div -->
    <div>
        <p> this is para </p>
        <b> this is bold text </b>
        <em> this is italic text </em>
    </div>
    ```

2. `<span>`:
    1. it is a container element, used to target a piece of content in the element.
    2. its generally used to styling purpose.
    3. its an `inline element` i.e, it occupies only the required width
    ```HTML
    <style> span{ color: red } </style> <!-- applies red color only to 'paragraph' in the <span> tag -->
    <p> this is a <span>paragraph</span> </p>
    ```
### List tags
There are three types of lists in html
1. ordered list
2. unordered list
3. description list

#### ordered list
1. in ordered list items appear with `numbers`
2. we use `<ol>` tag to create an ordered list.
3. each item in the list should be wrapped in `<li>` tag
```HTML
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
    <li>Item 5</li>    
<ol>
```

#### unordered list
1. in unordered list items appear with `bullet points`
2. we use `<ul>` tag to create an ordered list.
3. each item in the list should be wrapped in `<li>` tag
```HTML
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
    <li>Item 5</li>    
<ul>
```

#### description list
1. the description list is used in the scenerios where each item in the list has some definition.
2. we use `<dl>` tag  to create a description tag.
3. the description item is wrapped in `<dt>` tag and the definition is wrapped in `<dd>` tag
```HTML
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language<dd>

    <dt>CSS</dt>
    <dd>Cascading Style Sheet</dd>
</dl>
```

### Anchor tag - `<a>`
1. The `<a>` tag is used to create `hyperlinks` in HTML.
2. it is a container tag, the content will be displayed on webpage & when clicked on it, it navigates to corresponding `hyper referance (href)`
3. it allows us to navigate to 
    1. to a section on the same webpage using `id` & `#`.
    2. to a different page with in the same website (`relative links`)
    3. to any external websites (`absolute links`)
    4. or any `files` like `pdfs`, `images` etc 
4. Attributes for `<a>` tag:
    1. `href`( `important` & `mandatory` ): the url or path to link
    2. `target`: it tells where to open the linked document
        1. `_blank`: opens in a new tab
        2. `_self`: (default): opens in the same tab
    3. `title`: adds a `tooltip`text when hovered over the link.
    4. `download`: to download the document without opening it, (commnly used with files)
```HTML
<a href="github.com/sn0914r" target="_blank" title="github">view profile</a>
<!-- 
 1. the hyperlink is linked to 'github.com/sn0914r'.
 2. target is set blank, so it opens in a new tab
 3. title is github, so when the link is hovered it shows 'github' as a tooltip
  -->
```

### Media
#### `<img>`
1. `<img>` tag is used to insert images
2. Attributes for `img` tag:
    1. `src`: image path or link
    2. `alt`: the text about image( used for screen reader or rendered when image fails to load)
    3. `width`: sets the width of the image (`in px`)
    4. `height`: sets the heigth of the image (`in px`)
    5. `loading`: loading attribute decides when the image should be loaded
        1. `lazy`: delays loading until it's near the `viewport`.
        2. `eager`: loads the image `immediately`
        3. `auto` (default): brower decides when to load
```HTML
<img src="../assets/randomImage.jpg" alt="cow image" width="100" height="100" loading="lazy" >
<!--
1. the path of image is set to ../assets/randomImage.jpg
2. the value for 'alt' attribute is read by screen readers & it will be displayed on webpage when image fails to load.  
3. width and height set the dimesnions in pixels
4. loading is set lazy, so the image loads only when its near to viewport / visible area of webpage.
-->
```

#### `<video>`
1. the `<video>` tag is used to insert the `videos` in the webpage.
2. Attributes for `<video>` tag:
    1. `src`: path to local video
    2. `controls`: to add `play`, `pause`, `volume`, etc
    3. `autoplay`: to make video play automatically
    4. `loop`: to loop when it ends
    5. `muted`: to start with no sound (the video should be `muted` for `autoplay`)
    6. `poster`: to add thumbnail, it takes the image path as value.
    7. `width` & `height` : to set dimensions
3. the very old browsers don't support the  `<video>` tag. so to notiffy the user that there is a video but this brower doesn't support, we can add some `fallback content` between the video tags
```HTML
<video
    src="../assets/ben10_video.mp4"
    controls
    loop
    poster="../assets/randomImage.jpg"
    width="400"
    height="300"
>
    this browser doesn't support video tag
</video>
<!-- "this browser doesn't support video tag" this is the fallback content, this will be displayed when browser don't support the video tag -->
``` 
#### `<audio>`
1. The `<audio>` tags works same as `<video>` tag but for audio files
2. Attributes: 
    1. `src`
    2. `controls`
    3. `autoplay`
    4. `loop`
    5. `muted`
```HTML
<audio
    src="../assets/ben10.mp3"
    controls
    autoplay
    loop
>
this browser doesn't support audio tag
</audio>
```