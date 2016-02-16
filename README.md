# treemenu.js
treeMenu - simple jQuery plugin. Add togglers to ul > li > *  structure

## Example

http://xevinbox.github.io/treemenu.js/

## Usage

1. include jQuery
  ````
    <script src="jquery.min.js" type="text/javascript"></script>
  ````

2. include treeMenu script and styles in your document
  ````
    <script src="jquery.treemenu.js" type="text/javascript"></script>
    <link href="jquery.treemenu.css" rel="stylesheet" type="text/css" />
  ````

3. Attach treeMenu when the document is loaded
  ````
    <script type="text/javascript">
        $(document).ready(function(){
            $("ul.mytree").treemenu();
        });
    </script>
  ````
