presentation-javascript
=======================

Various JavaScripts related to HTML5 based presentations


code_highlight.js
-----------------

Can be used in combination with reveal.js to highlight individual parts of a code block as reveal fragments.

Example usage:

    <section>
        <pre>
            <code id="code1">code_line1
                code_line2
                code_line3
                code_line4
            </code>
        </pre>
        <div class="fragment" data-prettify="code1" data-prettify_lines="1:2">
    </section>

    <script>
        Reveal.addEventListener( 'fragmentshown', show_lines);
        Reveal.addEventListener( 'fragmenthidden', hide_lines);
    </script>

The effect can be seen in this [video](http://www.youtube.com/watch?v=v11oO5I8JgQ&feature=plcp)