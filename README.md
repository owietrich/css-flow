css-flow
========

CSS normal flow is often misunderstood and leads to a heck lot of junk in our code. Did you already applied different `position` or `display` to a given selector until you get one that works?

If the answer is yes, I invite you to read the rest of this article. 

## overview

So what is normal flow anyway? It is basically the way your elements will be rendered and will flow down a document if not [positionned](http://github.com/owietrich/css-positions).

Normal flow is part of the [basic box model](http://www.w3.org/TR/css3-box/) described in the HTML specificiations. You'll need to know at least 4 types of rendering box used for an element in order to master it:

  - block
  - inline
  - inline-block
  - none


This article is illustrated with concrete [examples](https://github.com/owietrich/css-flow/blob/master/examples).

## block

A `block` element will span the full width of its parent element and will start on a new line in the normal flow. The flow will always continue on a new line after the block element.

You can change the dimensions of a block element (`width` and `height`) in the normal flow.

In fact block elements are elements that are fomatted visually as block using `display` as `block`, `list-item`, `table` or `table-*`.


## inline

## inline-block

