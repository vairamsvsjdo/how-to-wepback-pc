Consider two elements one above the other each with padding of 1em. This padding is considered to be part of the element and is always preserved.

So you will end up with the content of the first element, followed by the padding of the first element, followed by the padding of the second, followed by the content of the second element.

Thus the content of the two elements will end up being 2em apart.

Now replace that padding with 1em margin. Margins are considered to be outside of the element, and margins of adjacent items will overlap.

So in this example, you will end up with the content of the first element followed by 1em of combined margin followed by the content of the second element. So the content of the two elements is only 1em apart.

This can be really useful when you know that you want to say 1em of spacing around an element, regardless of what element it is next to.

The other two big differences are that padding is included in the click region and background color/image, but not the margin.


Also you should take note that padding is included in total width/height the element, when used with box-sizing: border-box; so if you have width: 100px; padding-left: 20px; the total width will still be 100px but the area for content is reduce by 20px, unlike box-sizing: content-box; where padding is separate in calculating content width which makes your total width 120px in content-box; 
