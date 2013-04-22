JQuery Perspectives
===================

A JQuery plugin enabling users to dynamically view content according to one or
more perspectives.

How It Works
------------

Using perspectives is as easy as:

### 1) Include file:
```HTML
<script src="/path/to/jquery.perspectives.js"></script>
```

### 2) Tell the control widget where to attach.

```HTML
<div class="perspective-manager" />
```

### 3) Add perspectives.

```HTML
<div class="p">
  This text will be seen by everyone. <span data-perspective="coding">This
  is extra information for coders. </span>On to anether topic. <span
  data-perspective="coding operations">Mention something for coders and/or
  admins. </span>
</div>
<div class="p" data-perspective="coding&operations">
  Notice the '&amp;'? That means this paragraph is for viewers who have
  selected both the 'coding' and 'operations' perspectives.
</div>
```
