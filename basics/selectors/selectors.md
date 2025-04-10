## Selectors
#### Basic selectors
1. `*`: selects `all elements`.
2. `tagName`: selects all elements that matches the `tag name`.
3. `.className`: selects all elements that matchs the `class name`
4. `#idName`: select elemnt with specific `id`.
5. `selector1, selector2,..`: selects all elments matching any of the given selectors.

#### Combinators
1. `div.className`: selects `div` with given `class name`.
2. `div#idName`: selects `div` with given `id`.
3. `div p`: selects `p` elements in all levels from `div`.
4. `div *`: selects all type of elements inside the div.
5. `div + p`: selects one `p` tag after `div`.
6. `div ~p`: selects all `p` tags after `div`.

#### Attribute selectors
1. `selector[attributeName]`: selects all elements with given `attributeName`.
2. `selector[attributeName=value]`: selects all elements with given `attributeName` and `value`.
3. `selector[attributeName1=value1][attributeName2=value2][attributeName3]`: selects the elemnet that has all the listed `attributeNames` and `values`.