# Spacing

Generate any number of spacing classes based on a starting size.

## Installation

```
fonzie install spacing
```

## Usage

```scss
@import 'spacing';
@include generate-spacing-classes(10px);
```

The mixin `generate-spacing-classes` has two parameters

`$base`: The base size to use to generate the classes
`$n`: The number of spacing classes to generate.

You can then use these in your HTML

```html
<div class="padding-y-1">
  Foo
</div>
```

This would apply a padding top and bottom of 10 pixels. If we used the class `padding-y-2` it would be 20px.

You can use 3 types of classes; `padding`, `margin` and `outset`. Outset is just negative margin.