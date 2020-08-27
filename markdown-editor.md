---
title: Markdown Editor
pagetype: homepage
---

<link rel="stylesheet" href="editor.md/css/editormd.min.css" />
<div id="editor">
    <!-- Tips: Editor.md can auto append a `<textarea>` tag -->
    <textarea style="display:none;">### Hello Editor.md !</textarea>
</div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="editor.md/editormd.min.js"></script>
<script src="editor.md/languages/en.js"></script>
<script type="text/javascript">
    $(function() {
        var editor = editormd("editor", {
             width: "100%",
             height: "100%",
            // markdown: "xxxx",     // dynamic set Markdown text
            path : "editor.md/lib/"  // Autoload modules mode, codemirror, marked... dependents libs path
        });
    });
</script>