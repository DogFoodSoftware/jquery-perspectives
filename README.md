JQuery Perspectives
===================
An HTML5+JQuery plugin enabling users to dynamically view content according to
one or more perspectives.

Installation
------------
1.  [Grab the latest.](https://github.com/DogFoodSoftware/jquery-perspectives/archive/master.zip)
2.  Put the 'jquery.perspectives.js' file where the webserver can serve it.
3.  Include the plugin on your page:

    ```HTML
    <script src="/path/to/jquery.perspectives.js"></script>
    ```

Usage
-----
1.  Tell the control widget where to attach:

    ```HTML
    <div class="perspective-manager" />
    ```

2.  Add perspectives:

    ```HTML
    <div class="p">
      Text for everyone. <span data-perspective="coding">Text for
      coders. </span>On to another topic.
      <span data-perspective="coding operations">Mention something for coders
      and/or admins.</span>
    </div>
    <div class="p" data-perspective="coding&operations">
      Notice the '&'? This paragraph is visible when both the 'coding' and
      'operations' perspectives are selected.
    </div>
    ```
