# Box model
#### 1. borders
1. `border` is the short hand for `border-width`, `border-style`, `border-color`. 
2. The synatx is : `border: <thickness> <style> <color>`
3. `values`:
    - `<thickness>`: `<units>`
    - `<style>`: `solid | dashed | double | groove | none`
     `<color>` : colors
4. we can set the border for individual sides using the following props:
    - `border-top`
    - `border-bottom`
    - `border-left`
    - `border-right`
5. `border-radius`: It is used to make rounded corners for elments. It takes `<units>` as value.
6. we can make rounded corner at an indivial side using the following props:
    - `border-top-left-radius`
    - `border-top-right-radius`
    - `border-bottom-right-radius`
    - `border-bottom-left-radius`

#### 2. padding
1. `padding `: It allows us to adjust spacing inside the border.
2. `props` for targeting individual sides:
    - `padding-top`
    - `padding-bottom`
    - `padding-left`
    - `padding-right`
3. `short hand`
    - `padding`: `<top> <right> <bottom> <left>`
    - `padding` : `<top> <right & left> <bottom>`
    - `padding` : `<top & bottom> <right & left>`
    - `padding`: `<all sides >`

#### 3. margin
1. `margin `: It allows us to adjust spacing outside the border.
2. `props` for targeting individual sides:
    - `margin-top`
    - `margin-bottom`
    - `margin-left`
    - `margin-right`
3. `short hand`
    - `margin`: `<top> <right> <bottom> <left>`
    - `margin` : `<top> <right & left> <bottom>`
    - `margin` : `<top & bottom> <right & left>`
    - `margin`: `<all sides >`

#### 4. box sizing
1. Box sizing in controls how the total size of an element is calculated.
2. `box-sizing: content-box` (default):
    1. width and height apply only to content.
    2. padding and border are added after the given width/ height.
    3. so, total size = width + padding + border.
    ```Css
    div{
        box-sizing: content-box;
        width: 200px;
        padding: 10px;
        border: 5px solid green;

        /* here the width proportions are
            total width: 200px+10px+5px = 215px
            1. padding : 10px
            2. border : 4px
            3. width : 200px
         */
    }
    ```
3. `box-sizing: border-box` (default):
    1. width and height apply upto the border.
    ```Css
    div{
        box-sizing: content-box;
        width: 200px;
        padding: 10px;
        border: 5px solid green;

        /* here the width proportions are
            total width: 200px
            1. padding : 10px
            2. border: 5px
            3. content: 200-10-5 = 185px 
         */
    }
    ```