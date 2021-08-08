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