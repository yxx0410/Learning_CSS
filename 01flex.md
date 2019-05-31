flex: control items alignment and justification in a flex container

flex-container css property
1. display

2. flex-direction: row,column,row-reverse,column-reverse
change main axis and cross axis 

3. justify-content: flex-start flex-end space-between center space-around
how jusifity on main axis

4. align-items: flex-start flex-end center baseline stretch(default)
how align at cross axis

5. align-content: flex-start flex-end space-between center space-around stretch
if items all multi-line, and container height is higher than items total, manage each line justification

6. flex-wrap: wrap, wrap-reverse, nowrap
if items width in total more than container, allow items wrap to next line

7. flex-flow: flex-direction flex-wrap

flex-items properties

1. align-self
specify align at cross axis for item itself

2. no justify-self or justify-content,
2. use margin:auto to control 

3. flex-shrink: integar,0
set how item shrink if container width is lower than items' width in total, higher value shrink more
a group of same value items will equally share space left
higher more space, 0 don't change

4. flex-grow: integer,0
set how item contain the extra space. higher value get more space,
a group of same value items will equally share space left
higher more space, 0 don't change

5. flex-basis: auto, width
if items size is set, flex-basis is width, if size is not set, flex-basis is width of content

6. flex: flex-grow flex-shrink flex-basis, auto

usage:
how to display a group item horizon like nav, vertical like header content footer
use flex-grow flex-shrink flex-basis helps a lot 
