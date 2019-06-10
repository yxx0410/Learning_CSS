# box model

box model is foundation of layout of web page
each element is represent as a rectangular box
web page looks like consisted of many boxes

from outside to inside
margin border padding content
width height

## box-model property
box-sizing:border-box/content-box
width/height of box or conent
###- border-box
set width/height as box's entire width/height
height/width = padding + content
entire box width/height = width/height + margin + border

###- content-box
set width/height as content's width/height
height/width = content
entire box width/height = width/height + padding + margin + border

### hint
1. background extend to the edge of the border
but background_clip can change it
2. in border box, if content size (content + padding) is larger than box of width and height, scroll will apply
overflow property can control it 
3. box height default adopts the height of the content, unless absolute height set
4. border-box prefered, but chrome is set content-box default
5. border-box, if padding is larger than width and height,
box will be extended

## relative property

### overflow
at border-box, if content + padding size larger than box size, content will be overflowing
overflow: hidden, hide the content that overflows the box (default)
overflow: visible: overflowing content is shown outside of the box
overflow: auto: overflowing is hidden, but scroll bars are shown to control the box content

### background-clip
how background extends in the box
background-clip:border-box: to border edge
background-clip:padding-box: to padding edge
background-clip:content-box: to content edge

### outline
like of border outside border, inside margin

## box type
display property set box type
1. block
block box contains seperate line, whole box model applied to block boxes

2. inline
inline box flows with document's text
width and height settings have on effect on inline boxes
margin border set on inline boxes will update the position of surrounding text

3. inline-box
between inline and box
flows with surronding text,
but it can be sized using width and height

4. hint
1. block always contains whole line
2. inline box has no enough space, will wrap to next line the overflow part
3. inline box has no enough space, it will show at next line with entire part