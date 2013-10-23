# Atomic components: arrange

Component for arranging/aligning horizontal cells, a bit like flexbox.

Read more about [Atomic framework](https://github.com/atomic-css/atomic).

## Installation

* [__Bower:__](http://bower.io)
  `bower install --save atomic-css-components-arrange`
* [__Component(1):__](http://component.io)
  `component install atomic-css/components-arrange`
* __Download:__
  [zip](https://github.com/atomic-css/components-arrange/zipball/master),
  [tar.gz](https://github.com/atomic-css/components-arrange/tarball/master)
* __Git:__ `git clone https://github.com/atomic-css/components-arrange.git`

## Available classes

* `Arrange` - core component class
* `Arrange-sizeFit` - descendant class for cells to snap to fit their content
* `Arrange-sizeFill` - descendant class for cells to expand to fill the
  remaining space
* `Arrange--middle` - modifier class for middle-aligned cells
* `Arrange--bottom` - modifier class for bottom-aligned cells
* `Arrange--equal` - modifier class for equal-width cells

## Extensions

### `arrange.gutter.css`

Modifiers for creating horizontal gutter between arrange items.

* `Arrange--gutter<Size>` - horizontal gutter of `<Size>` size

Where size `<Size>` can be:

* `Small` (5px)
* `Medium` (10px)
* `Large` (20px)

## Usage

Like many Atomic components, `atomic-css-component-arrange` relies on a base
component class that is extended by any number of additional modifier classes.
This component works best for small-scale UI layout, for example, image-content
pairs:

```html
<div class="Arrange">
  <div class="Arrange-sizeFit">
    <img src="img.png" alt="">
  </div>
  <div class="Arrange-sizeFill">
    Lorem ipsum dolor sit amet.
    …
  </div>
</div>
```

Or for an equally spaced row of buttons or icons, etc.

```html
<ul class="Arrange Arrange--equal">
  <li class="Arrange-sizeFill">
    <button class="Button Button--full">Reply</button>
  </li>
  <li class="Arrange-sizeFill">
    <button class="Button Button--full">Like</button>
  </li>
  <li class="Arrange-sizeFill">
    <button class="Button Button--full">Save</button>
  </li>
  <li class="Arrange-sizeFill">
    <button class="Button Button--full">Remove</button>
  </li>
</ul>
```

N.B. This component affects the width of images in cells.

## Requirements

* Sass 3.2+

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 8+