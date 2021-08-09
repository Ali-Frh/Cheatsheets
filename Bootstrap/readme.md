# Bootstrap Cheatsheet

REMs Measurement System<br/>
16px = 1rem (Default)

## Typography
BS Classes such as:
- h1-h6 class => heading tags
- small class => html5 ```<small>``` Equivalent
- display-[1-4] class => Sexy thin Heading Text
- lead class => Paragraph Equivalent
```html
<p class="h1">Heading</p> (<h1>Heading</h1>)
<span class="small">خ</span> (<small>خ</small>)
<h1 class="display-4">Penis</h1>
<p class="lead">lorem ....</p>
```
### Text stuff
#### Transitions:
- text-left | text-center | text-right
Makes LTR,Center,RTL
- text-uppercase | text-lowercase | text-capitalize <br/>
Makes UPPERCASE,lowercase and Capitalize
- font-weight-bold | font-italic | font-weight-normal | font-weight-light
- text-justify

#### Text/BG Color
Use Colors as text-color or bg-color:<br/>

- primary => High Blue
- secondary => Gray
- success => Green
- danger => RED
- info => Light Blue
- light => Almost White
- muted => Light Gray #Just For Text (not bg)
- white => White

### Breakpoints
xs < 576px <= sm < 768px <= md < 992px <= lg < 1200px <= xl <br/>
for example (text-center)
```html
<h1 class="text-md-center"> خ </h1>
```
for dudes who their screens is md or larger, heading will be appeared in center

### Floats and Positions:
- float-[left/right] class<br/>
makes object stick to the side
- clearfix class <br/>
fixes background issue of fixed object's parents
- fixed-[top/bottom] <br/>
always stay at top/bottom
- sticky-[top/bottom] <br/>
stick to top when you passed away it, but back to it position when scrolls back before its place.

### CSS Flex Box
- css display: **flex**; means all child elements in a row
- css display: **inline-flex**; means like previous one but container alloc just required space
- css flex-direction:<br/>
    **row** (default) means LTR <br/>
    **row-reverse** means RTL <br/>
    **column** means up to down <br/>
    **column-reverse** means bottom to top <br/>
- css flex-wrap: [wrap/nowrap] means item wrapping during low screen width
- css flex-flow: [direction wrapstate], this property is a mix of flex-direction and wrap
- css justify-content: <br/>
        **flex-start** means main axis <br/>
        **flex-end** means not main axis<br/>
        **center** means place at center<br/>
        **space-between** means fills all space <br/>
        **space-arround** means like *space-between* but first and last item hasnt attached to the edge of screen<br/>
        **space-evenly** means all spaces (between and arround) are equal  <br/>
 - align-items:<br/>
        **stretch** (Default) means it streched from flex-start to end <br/>
        **flex-start** means elements align at start of cross axis <br/>
        **flex-end** means elements align at end of cross axis <br/>
        **center** means elements align at middle of cross axis <br/>
        **baseline** means Texts of elements are Aligned from bottom in a hypothethical line <br/>
 - align-content: Just Like align-items Properties.
 - order: default is **0**, anything < 0 will be first and bigger than 0 is last one.
 - align-self: override align of container by the element
 - flex-grow: default is **1**, its growing speed when screen bigger, flex-wrap interfer it
 - flex-shrink: opposite of flex-grow
 - flex-basis: **as px**, if flex-direction is row, its width and if dir is column, its modify height of element
 - flex: [flex-grow flex-shrink flex-basis] mix of three of them