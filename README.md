[![Build Status](https://travis-ci.org/jshcrowthe/iron-drag-drop.svg?branch=master)](https://travis-ci.org/jshcrowthe/iron-drag-drop)
[![Coverage Status](https://coveralls.io/repos/github/jshcrowthe/iron-drag-drop/badge.svg?branch=master)](https://coveralls.io/github/jshcrowthe/iron-drag-drop?branch=master)
# iron-drag-drop 

### &lt;iron-drag-drop&gt;

An element for creating a drag-n-drop region on the page

On its own, this element has **no DOM** it is used to
wrap existing markup to create a droppable region

Example:
```html
<iron-drag-drop>
  <h2>Hello iron-drag-drop</h2>
</iron-drag-drop>
```

You can also provide DOM to be used in an overlay that
triggers when a file is dragged over the drop area. You
do so by providing an element with the attribute `overlay`


Example:
```html
<iron-drag-drop>
  <div overlay>
    <h1>This will only display when someone is dragging over the drop area</h1>
  </div>
  <h2>This will display ALL the time and constitutes the droppable area</h2>
</iron-drag-drop>
```

### Styling
`iron-drag-drop` provides several CSS mixins/properties to allow for customization of 
different regions within the component.

Custom property | Description | Default
----------------|-------------|----------
`--iron-drag-drop-border` | The default border styles | `2px solid transparent`
`--iron-drag-drop-border-dragging` | The border styles when a files is by dragged over the drop area | `2px solid #B9B9B9`
`--iron-drag-drop-overlay` | A mixin that allows a user to customize the overlay area as they wish | `{}`
