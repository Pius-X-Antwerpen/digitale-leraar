---
title: Markdown Editor
pagetype: homepage
---

## Wat is markdown?

Markdown is een manier om tekst aan te duiden als titel, tekst, afbeelding, ... Zo schrijf je bijvoorbeeld een `# ` om aan te duiden dat iets een titel is, of `## ` om aan te duiden dat iets een subtitel is.

Hieronder kan je aan de linkerkant tekst typen en opmaken met de knoppenbalk, en rechts het resultaat bekijken.

Schrijf je artikel gerust in deze editor, waarna je de Markdown tekst kan kopieren en plakken op de juiste plek in Github.

Vergeet niet de title, authors en tags in te vullen! Een tag is een zoekterm die ook gebruikt kan worden om je artikel te vinden.

<link rel="stylesheet" href="editor.md/css/editormd.css" />
<div id="editor">
    <!-- Tips: Editor.md can auto append a `<textarea>` tag -->
    <textarea style="display:none;">---
title: Markdown Editor

authors: 
 - Joske Vermeulen

tags:
 - markdown
 - artikel schrijven
---

## Wat is markdown?

Markdown is een manier om tekst aan te duiden als titel, tekst, afbeelding, … Zo schrijf je bijvoorbeeld een # om aan te duiden dat iets een titel is, of ## om aan te duiden dat iets een subtitel is.

Een lijstje is zo simpel als een `-` voor elk lijst-onderdeel te plaatsen. Of je kan met `1.`, `2.`, ... werken om een genummerd lijstje te maken.

 - zo dus
 - bijvoorbeeld

Hier kan je aan de linkerkant tekst typen en opmaken met de knoppenbalk, en rechts het resultaat bekijken.

Schrijf je artikel gerust in deze editor, waarna je de Markdown tekst (dus de linkerkant) kan kopiëren en plakken op de juiste plek in Github.

Vergeet niet de title, authors en tags in te vullen! Een tag is een zoekterm die ook gebruikt kan worden om je artikel te vinden.
</textarea>
</div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="editor.md/editormd.min.js"></script>
<script src="editor.md/languages/en.js"></script>
<script type="text/javascript">
    $(function() {
        var editor = editormd("editor", {
             width: "100%",
             autoHeight : true,
            path : "editor.md/lib/",  // Autoload modules mode, codemirror, marked... dependents libs path
            toolbarIcons : function() {
                return editormd.toolbarModes["simple"];
            }
        });
    });
</script>