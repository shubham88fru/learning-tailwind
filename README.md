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

.inline-block {
} /*display: inline-block*/

.rounded-full {
} /*cirulare border*/

.divide-y {
} /* add a line between the child elements.*/
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

.flex-col {
} /* change flex-direction: column*/

.grow {
} /* flex-grow: 1*/
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

# 7. Styling buttons: Element states and transitions.

```css
.hover:text-blue-600 {
} /*on hover, change text to blue 600*/

.hover:underline {
} /*on hover, underline*/

.transition-colors {
} /*transition the color*/

.duration-300 {
} /*set transition duration to 300ms*/

.focus:outline-none {
} /*in focus state, set outline to none.*/

.disabled:cursor-not-allowed {
} /*remove the cursor pointer from button if it is in disabled state*/
```

# 8. Reusing styles with @apply

```css
/**
    create a self defined css class `input` (can use this in the class attribute of html element) which is simply a group of 
    bunch of classes applied together (see below). This is a neat
    trick for reusing styles.
*/
@layer components {
  .input {
    @apply w-full rounded-full border px-4 py-5 text-sm
        transition-all duration-300;
  }
}
```

# 9. Absolute positioning, z-index etc.

```css
.absolute {
} /* equivalent to position: absolute */

.inset-0 {
} /* top: 0; left: 0; right: 0; bottom: 0;*/
```
