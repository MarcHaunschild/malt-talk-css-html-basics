# malt academy Talk "Basics of HTML and CSS"

![alt text](https://raw.githubusercontent.com/MarcHaunschild/malt-talk-css-html-basics/master/assets/300420_Basics_HTML_CSS_EN.png "Logo Title Text 1")


Here you find the source code from the Malt academy talk "Basics of HTML and CSS"

** CHANGE in the HTML-Document after the talk! **

I wanted to place the element `aside` next to `main`.

So need it to be a sibling of `main` - so I took the `aside` element out of main and put it after `main`.

Do this in your own project only, if it makes sense. Because HTML is all about sense and meaning.

By the way: if the `aside` can stay in the `main` element, make the `main` a grid conatiner. Everything in body does not have to be placed in a grid, anyway all the other elements are standing on top of each other.

This is the reason why I have to give all children of body the style `grid-colum: 1 / 3;` 

This tells the browser to place an element from line one to line three of the grid. Line one is before the first column, line two is between column one and column two and line three is after column 2 (and before column three. if there is a thir column).

So `1 / 3` means column 1 and 2.

See also https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column

While talking it did not work, because I wrote `0 / 2` - for a reason I don't understand myself, I thought I have to start counting at 0...

Of course on a real life web page, the main article would be wider than the sidebar, so try playing around with the fraction values in line 4 of the css file.

Think of them as a ratio between the elements in each row. If you write `5fr 2fr` for example this means that the first row gets 5 parts of the whole and the second row will get 2 parts.

If you want something behaving like on a bootstrap grid, you need the sum of the fractions to equal 12 like so: 8fr 4fr

But you already can see in this little example, that you have much less constraints than in a bootstrap layout, not even mentioning, that css grid is smart, whre bootstrap is dull like a stone. Because with css grid you can make responsive layouts without media queries. If you are interested in this feature of css grid, search the Mozilla developer Network for autofill and  autofit.

By the way. you are free to combine css grid and flex: put a flex container into an grid item and enjoy the magic!

Heve fun!