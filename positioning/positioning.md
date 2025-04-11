### Positioning
1. Positioning allows us to `control where an element appears` on the webpage.
2. The `position` property is used to set the `positioning type` & `top`, `bottom`, `left` & `right` is used to move the element.
3. values for `position` prop:
    - `static`: 
        1. it is the default value, it places the elements in the normal document flow (left to right).
        2. it `ignores` `top, bottom, left & right` props.

    - `relative`: 
        1. it places the element in the normal document flow (just like static)
        2. it `accepts` `top, bottom, left & right` props to move the element.
        3. when moved, it still occupies its original space in the layout (others don’t shift).

    - `absolute`: 
        1. it removes the elemnt from the document flow (stacks on the webpage like layer).
        2. And positioned relative to the nearest positioned parent with postion `relative`, `absolute` or `fixed`.
        3. it `accepts` `top, bottom, left & right` props to move the element from the relative parent.
        4. if no relative parent found, it will use the viewport as reference.
        5. Usecases:
            - Dropdown menus under buttons or navbars
            - Tooltips near buttons or icons
            - Modals or popup boxes (centered or placed freely)
            - Notification badges on top of icons

    - `fixed`:
        1. the element is removed from the normal document flow (like absolute).
        2. it is positioned relative to the browser window (viewport), not any parent.
        3. it stays in the same place on the screen even when you scroll.
        4. it accepts `top, bottom, left, and right` to place the element anywhere on the screen.
        5. Use cases: 
            - Sticky headers or footers
            - Chat buttons
            - Scroll-to-top buttons
            - Floating menus

    - `sticky`:
        1. sticky is a `mix of relative and fixed positioning`.
        2. it starts like relative (part of normal flow).
        3. but when you scroll up, it "sticks" to a set position with `top`, `left`, etc(like fixed).
        4. it will stick only while its parent is visible on the screen, otherwise vanishes.
    
### z-index
1. z-index controls the stacking order of elements like which one appears on top when elements are layered.
2. higher the z-index, above the elment will be.
3. It only works with `positioned` elements like `relative`, `absolute`, `fixed`, `sticky`.