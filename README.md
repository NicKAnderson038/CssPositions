# CSS - Positions

- [Position Absolute]('#position-absolute')
- [Position Relative]('#position-relative')
- [Position Fixed]('#position-fixed')

#

#### Position Absolute

This will place the elememnt relative to the containing elemnt.

```bash
    position: absolute; top:0; left0;
```

The element will move within the containing element (in this case a `<html>` element wrapping the document). However, if the parent containing element is a `position:absolute`. Then the child will match this vs. the document parent level containing element.

\*\* Think of this position as a plot point on a graph. This is a exact location.

#

#### Position Relative

Think of this position as moving away from top, right, bottom, left. If you say `top:50px` then you'd move down 50px relative to the container. So your already considered at `top:0` and `left:0`by default.

#

#### Position Fixed

Very similar to `position:absolute` but ALWAYS reffers to the view port.

Other Special Features.

1. It's important to note that charactistics of parent elements between the `position:fixed` element and view port will effect it. Like a parent `<div>` that contains `padding: 10px`. This will push it somewhat from where you'd want it within the view port.

2. When scrolling, the `position:fixed` element will remain in the same spot. Example: perminate header or footer abilitiy.