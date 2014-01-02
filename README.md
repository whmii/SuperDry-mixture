# SuperDry

SuperDry is a boilerplate workflow for use with Grunt Sass and Autoprefixer!
Incorporated modules include structure from Sassaparrilla and Normalize as well as an abstraction Foundation 5 mixin-based media quires and grid system.

SuperDry also contains ResponsiveSlides.js for a quick slide-show implementation. Because who doesn't love a slideshow.

SuperDry is designed to be a tight and focused implementation that can be rapidly built upon and scaled.

## Components

Component = factor + ratio

### Factor

The default factor for components is 0, meaning that no multiplier is applied. If factor is greater than 1 it is assumed that this is a factor multiplier. Values entered multiply the factor. It is encouraged that whole numbers are entered for this value as it is meant to represent levels (i.e. level 1, level 2, level 3, etc) 

If negative values (-) are entered, these act as a negative multiplier and will reduce the padding of the component linearly at half the rate of posture factors. Alternatively, decimal values can also be entered but this functionality may be deprecated.

The base value for components is the grid-margin since it is assumed that this value will be the same as the horizontal padding (in most cases).

### Ratio

The ratio is then used to convert the grid-margin value in to the vertical padding and margin. 

The ratio base is derived from grid-margin / line-height. This defaults to 0.8 meaning that the vertical-padding will be 80% of the horizontal-padding, great for alerts and buttons. The ratio can be directly modified by entering a numeral value in to the mixin. For example entering a value of 1.5 will make the object's padding 1.5X taller than it is wide, perfect for items like panels and v-cards.

While vertical-margins are on by default, this can be manipulated in the mixin. Setting 'false' or '0' will make the object have 0 vertical-margin. Setting 'auto' will cause the vertical-margins to be undeclared. Additionally, 'top' and 'bottom' can also be entered which limits vertical margin to one direction or the other.

### Assorted Components

While base styles for items like buttons and panels have been added, they are primarily placeholders and not meant as complete patterns. Much of the purpose of SuperDry is infrastructure.

----------------------------

## Ref

* http://foundation.zurb.com/docs/components/grid.html
* http://responsiveslides.com/
