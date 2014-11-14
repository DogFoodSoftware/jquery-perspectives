JQuery Perspectives
===================
An HTML5+JQuery plugin enabling users to dynamically view content according to
one or more perspectives. Use `data-perspective` to specify the nature of the
content. E.g., embed and interleave 'developer' and 'sysops' notes in the same
document while allowing viewers to focus on the information they need.

Limitations
-----------
The current implementation is limited to a single perspective choice. The next
version will include the ability to enable multiple perspectives at once. The
perspective content specification is considered complete.

Installation
------------
### For Kibbles Projects

JQuery Perspectives is included in the standard Kibbles distribution.

### For Any Project

1.  [Grab the latest tarball](https://github.com/DogFoodSoftware/jquery-perspectives/archive/master.zip)
    and extract it
2.  Copy 'src/lib/jquery.perspectives.js' file where the webserver can serve it.
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

<!--
Thanks to clintel for demonstrating how to combine fenced code with ordered
lists:

https://gist.github.com/clintel/1155906
-->
