# Museum-Of-Illusions

The Idea:
Try and guess the code/ how it was made.
(Basically it looks complex but it is simple with a hint of cleverness and creativity)

In coding specifically, creativity is highly valuable,
because creativity in some sense means to find an effecient and clever solution
to any unforseen issue

-OVERVIEW:
A museum of illusions is a place where creativity is value.
Paintings are mere canvases on a wall, but art is a story,
Time and effort are crucial in life, but art never relies on them, it is the authentic ability to create that is praised not the patience of creating.
In a museum, creativity is what seperates pieces, the tie breaker.. 
And much like other museums,
The museum of illusion is my safe place, where i tried to venture into creating something new.
And that's what makes it valuable.. for me.


-Technicalities:

HTML: (The canvas)
Nothing much to talk about a canvas, but without it, art would cease to exist.

CSS: (The paint)
from visual illusions to beautiful animation.
this project really improved my understanding of keyframes and animation properties.

-From css2 i learned:
  using the :nth-child()
  and learning an=bout its "even attribute"
  which means that the css onlu affects every second child.

-From css3 i learned:
  using 2 dimensions X and why in the transform property to move and rotate an object.
  And getting curious about the third Z dimension and started to research:
    "transform-style: preserve-3d;" property which adds translateZ() and rotateZ() attributes to the transform property.

-From css4:
  i trained and improved my grid optimization and customization skills from webdev3
  i learned that hover can be used to alter functional properties as well, not just visual ones.
  So i used my creativity and made the boxes snap immediately on hover and then return slowly after that to their original state.

JS:
The functionality and the interactivity,
the embodiment of creativity.

From js1 i learned: (A LOT):
  "canvas.getContext('2d')" which makes a canvas customizable,
  basically gives the developer the ability to alter, add or customize shapes and colors on the canvas.
  Lists/arrays: "dots = []", (Which made me relate between my js and python knowledge) 
  Dictionaries: "mouse = { x: -1000, y: -1000, radius: 260 }" (Similarly)
  Appending to a list "dots.push({ x: x, y: y })"
  Accessing the mouse coordinates "'mousemove', function (event) {mouse.x = event.clientX; ...}"
  which adds a .clientX property to the "event" attribute that describes the mouse coordinates.
  ".clearRect" to empty the canvas
  And some math "dist = Math.sqrt(dx * dx + dy * dy)" to calculate distance.
  conditions "if (dist < mouse.radius)" to make sure that only dots in the radius are affected.

From js2 i learned:
  Mostly about optimization and for loops,
  mixed with conditionals.
  The ability to create elements "cell = document.createElement('div');"
  and to control the inheritance of said elements. 

  WOW i was actually amazed when i found these in my research.

RESPONSIVENESS (I focused most on this part)

1. Media query
   Line 132: @media (max-width: 900px)
   When the screen gets narrower than 900px:
   - the .stage padding gets much smaller, so the content has more room
   - the side navigation boxes shrink from 150px to 110px
   - the Home button shrinks from 180px to 120px

2. clamp()
   Line 59: font-size: clamp(1.4rem, 4.2vw, 4.5rem) on the home title.
                    (lower-bound, variable, upper-bound)
   The title grows and shrinks with the window width, but it never gets
   smaller than 1.4rem or bigger than 4.5rem. 
   (1rem = 16px by default)

3. min-height, max-width and similar
   - line 4: min-height: 100vh on the body, so the page always fills the screen
     but can still grow if there's more content
   - line 93: max-width: 520px on .caption, so the text doesn't stretch too wide
     on big screens, but can still get narrower on small ones

4. vw units
   - vw: line 59 (4.2vw, the flexible middle value inside clamp())

5. Relative unit %
   - %: line 120 (left: 50%) together with translateX(-50%) on lines 121 and
     130 keeps the Home button centered no matter how wide the screen is

6. Flexbox
   - lines 51-54 (.home): a column flex layout that keeps everything centered
   - line 72 (.row): display: flex with flex-wrap: wrap, so the buttons drop
     onto a new line when there isn't enough space. This is why the fixed
     190px buttons (line 73) still fit on small screens.
   - lines 79-82 (.stage): column flex that centers the content on the
     showcase pages
   - lines 101-102 (.nav-left, .nav-right): column flex that stacks the
     navigation buttons

Extra:
- line 9: overflow-x: hidden on the body stops sideways scrolling caused by
  the big blurred blobs (lines 19-20)
- A dark island behind the text in js1 to improve readablity.

__In Summary__

I was amazed after realizing that JS is a highly convinient and VERSATILE.
And I could translate my python knowledge into JS.

For some reason, i thought js was only limited to webdevelopment,
but i was proven wrong. 
And That Fills Me With Joy and Anticipation.
