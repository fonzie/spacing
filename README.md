# Spacing

Generate any number of padding and margin classes based on a list of sizes.

## Installation

```
bower install fonzie-spacing
```

## Usage

```scss
@import 'fonzie-spacing/index';
@include fz-SpacingClasses($sizes: 10px 20px 40px);
```

The mixin `fz-SpacingClasses` has three parameters

`$sizes`: The base size to use to generate the classes
`$prefix`: Prefix all classes, default is `fz-`
`$suffix`: Add a suffix to every class. Default is `""`.

You can then use these in your HTML

```html
<div class="fz-py-1">
  Foo
</div>
```

In this case it will add 10px padding to the top and bottom of the element.

It generates these classes:

* p = Padding
* py = Padding top and bottom
* pz = Padding on the left and right
* pt = Padding top
* pb = Padding bottom
* pl = Padding left
* pr = Padding right

It will also generate the same margin classes for each size, but uses `m` instead of `p`.