# learning-tailwind

# 1. Colors classes.

```css
.text-yellow-400 {
} /*font color to yellow*/

.bg-yellow-500 {
} /*background color to yellow*/
```

# 2. Text styles

```css
.text-center {
} /* center the text.*/

.text-xl {
} /* large text.*/

.text-[120px] {
} /* font size of 120px*/

.font-semibold {
} /*font weight to 600*/

.uppercase {
} /* make the text uppercase*/

.tracking-[.35em] {
} /* for letter spacing of .35em*/
```

# 3. The box model: Spacing, Borders, and Display.

```css
.h-4 {
} /*height of 4rem*/

.h-screen {
} /*height:100vh*/

.w-72 {
} /* width equal to 18rem*/

.mb-4 {
} /*margin bottom of 1rem. 1rem = 16px*/

.px-4 {
} /* left and right padding of 1rem*/

.p-4 {
} /* padding of 1rem in all directions.*/

.border-b-2 {
} /* border bottom of 2 px*/

.border-stone-500 {
} /* border color stone*/

.space-x-4 {
} /* add a space of 1rem betwen children elements.*/

.hidden {
} /*display none*/

.overflow-scroll {
} /*overflow:scroll*/

.max-w-3xl {
} /*add a max width style.*/

.mx-auto {
} /* margin left and right (i.e. along x) to auto*/
```

# 4. Responsive design (Media queries)

```css
/*
    Tailwind has following media query breakpoints (by default).

    1. `sm` -> min-width: 640px
    2. `md` -> min-width: 768px
    3. `lg` -> min-width: 1024px
    4. `xl` -> min-width: 1280px
    5. `2xl` -> min-width: 1536px

    We can apply these prefixes to any css class in
    tailwind to change when those styles should trigger.
    Note that, in tailwind, adding a prefix `sm` doesn't mean that the style will only apply to small screens. Instead it means that the style would apply if the width is equal or above 640px. Similarly, for all other media query prefixes.
    The unprefixed classes will always apply and as soon as width goes above a media queries threshold, the prefixed version of that class (if applied) will override the unprefixed version.
    Remember, Tailwind is mobile first.
*/
.sm:my-16 {
} /* if width is sm and beyond (i.e. 640px) then margin in y direction be 4rem.*/
```

# 5. Using flexbox

```css
.flex {
} /*equivalent to display:flex --> setup a flexbox container*/

.items-center {
} /*equivalent to align-items:center --> vertically algin items*/

.justify-between {
} /*equivalent to justify-content:space-between*/
```

# 6. Using CSS Grids

```css
.grid {
} /*display:grid*/

.grid-rows-3 {
} /*a grid with 3 rows*/

.grid-cols-2 {
} /*grid with 2 cols*/

.gap-4 {
} /*grid gap of 1rem (16px) between columns*/

.grid-rows-[auto_1fr_auto] {
} /*grid-template-rows: auto 1fr auto;*/
```
