css-flow
========

CSS normal flow is often misunderstood and leads to a heck lot of junk in our code. Did you already applied different `position` or `display` to a given selector until you get one that works?

If the answer is yes, I invite you to read the rest of this article. 

## basics

So what is normal flow anyway? It is basically the way your elements will be rendered and will flow down a document if not [positionned](http://github.com/owietrich/css-positions).

Normal flow is part of the [basic box model](http://www.w3.org/TR/css3-box/) described in the HTML specificiations. You'll need to know at least 3 types of rendering box used for an element in order to master it:

  - block
  - inline
  - inline-block


This article is illustrated with concrete [examples](https://github.com/owietrich/css-flow/blob/master/examples).

### block

A `block` element will span the full width of its parent element and will start on a new line in the normal flow. The flow will always continue on a new line after the block element.

![block](/assets/block.png)

You can change the dimensions of a block element (`width` and `height`) in the normal flow.

In fact block elements are elements that are fomatted visually as block using `display` as `block`, `list-item`, `table` or `table-*`. You'll also format an element into a block using `float`, positions `absolute` or `fixed` and `overflow`.

### inline

At the opposite of block elements, inline-level boxes are displayed in lines and doesn't break the flow on a new one.

![inline](/assets/inline.png)

You can't change the dimensions (`width` and `height`) or an inline element.


### inline-block

Too often overlooked the `inline-block` is probably the most useful type of box. An inline-level element is a box which is flowed as a single inline box (the content is formatted as a block and the box itself is formatted aas an inline box).

![inline-block](/assets/inline-block.png)

To display block elements one next to an other, I would advise you to use `inline-block` instead `float` which is not suited for layouts (a floating element is not in the flow).


## flows and boxes

To finish this article, I just wanted to illustrate the type of boxes in a single example and how straightforward it is to create complex layouts:

![mix](/assets/mix.png)


