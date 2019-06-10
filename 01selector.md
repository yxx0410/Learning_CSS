# selector

how css connect to html element

## simple selector
 element
.classname
/# id

## atribute selector 
Presence and value attribute selectors and Substring value attribute   selectors.

### Presence and value attribute
[attr]
[attr=value]
[attr~=value]
often used in input or data-* custom attribute

### Substring value attribute selectors
match attribute value as regExp way
[attr^=val] starts with val
[attr&=val] ends with val
[attr*=value] contains val

## pseudo-classes

### pseudo for a element's state
a :active/:hover/:link/:visited

### pseudo for input
input :default/:checked/:disabled/:enabled/:focus/:valid/:invaild/:in-range/:indeterminate/:optional/:out-of-range/::placeholder/:read-only/:read-write/:required

### pseudo for child 
any :first-child/:last-child/:nth-child(n)/:nth-last-child(n)/:only-child

### pseudo for child based on type
any :first-of-type/:last-of-type/:nth-of-type(n)/:nth-last-of-type(n)/:only-of-type

### pseudo for p (text)
p :empty/:lang/

### other
:root/::selection/:target

## pseudo-element
position of an element
:: after
:: before
::first-line/::first-letter/

## combinators and selector lists
group - A, B - A and B selector follow same rules
descentdant - A B - only B as descentdant of A follow the rule
child - A > B - only B as direct child of A follow the rule
sibling - A ~ B - all B as the sibling of A follow the rule
following sibling - A + B - only B as the adjacent next element of A follow the rule
