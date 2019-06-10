# cascade and inheritance

cascade determines which selector effects on style
inheritance give child parents style

## cascade
1. important: property:value !important always win cascade. but never use it 

2. specificity- selectors' score
- inline style 1000
- id selector 100
- class selector 10
- attribute, psedudo-class 10
- element selector 1

when specificity is same, latest one takes effects

## inheritance
some property values apply to an element will be inherited by thtat element's children

most of inherited property is related to text
text-
list-
font-
table-
word-
color(text-color)
line-height
letter-spacing
white-space
cursor
visibility

all other not inherited like margin about size

property:inital/inherit/unset/