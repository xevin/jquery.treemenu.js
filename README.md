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
    <link href="jquery.treemenu.css" rel="stylesheet" type="text/css">
  ````

3. Create tree
  ````
  <ul class="mytree">
      <li><a href="/transport/">Transport</a>
          <ul>
              <li><a href="/transport/hovertanks">Hover tanks</a></li>
              <li><a href="/transport/quadbikes">Quad bikes</a></li>
              <li><a href="/transport/ecars">Electro cars</a></li>
          </ul>
      </li>
      <li><a href="/weapons/">Weapons</a>
          <ul>
              <li><a class="active" href="/weapons/knives">Knives</a></li>
              <li><a href="/weapons/grenades">Grenades</a></li>
              <li><a href="/weapons/lasers">Lasers</a></li>
          </ul>
      </li>
      <li><a href="/suits/">Suits</a></li>
  </ul>
  ````

3. Attach treeMenu when the document is loaded
  ````
    <script type="text/javascript">
        $(document).ready(function(){
            $("ul.mytree").treemenu();
        });
    </script>
  ````

## Options
  * delay - open/close animation delay. Default == **0**
  * openActive - open all trees that contains element with *activeSelector* class. Default == **false**
  * closeOther - at opening some tree, the other will be closed. Default == **false**
  * activeSelector - class selector name for active elements. Default == **'.active'**

Use options:
  ````
  $("ul.mytree").treemenu({
    'delay': 300,
    'closeOther': true,
    'activeSelector': 'active',
    'openActive': true
  });
  ````
