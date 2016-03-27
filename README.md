# css3-flexbox-grid
A lightweight grid system based on CSS3 Flexbox

Flexbox is a new layout mode in CSS3, it consists of flex containers and flex items.

The grid system uses similar syntax than bootstrap to make it easy th switch.


  **Versions:**
    
    - flexbox-grid.css -> 12 Units per row, Media Queries 500, 750, 1000
    - flexbox-grid.min.css -> same as flexbox-grid.css but compressed
    - flexbox-grid-24units.css -> 24 Units per row, Media Queries 500, 750, 1000    
    - flexbox-grid-24units.min.css -> same as flexbox-grid-24units.css but compressed    

  **Constants:**

    - $browser-context      -> Defines the default pixel size
    - $row-max-width        -> Defines the number of units a grid row can contain
    - $col-{a}-breakpoint   -> Defines the breakpoint for a specific media query

  **Media queries:**

    - col-{b}      -> grid columns independent from media query
    - col-xs-{b}   -> "extra small"    0px - $col-xs-breakpoint
    - col-sm-{b}   -> "small"          $col-xs-breakpoint - $col-sm-breakpoint
    - col-md-{b}   -> "medium"         $col-sm-breakpoint - $col-md-breakpoint
    - col-lg-{b}   -> "large"          $col-md-breakpoint - unlimited

  **Row Options:**

    - row-{a}                       -> Multiple lines, items will automatically move
                                       to new line when $row-max-width is exceeded

    - row-{a}-no-wrap               -> Single line, items can overlape on x axis and
                                       don't move to next line when $row-max-width is exceeded

    - row-{a}-items-flow-x-{b}      -> Defines the item alignment along the x axis (main axis)

    - row-{a}-items-flow-y-{b}      -> Defines the item alignment along the y axis (cross axis)

    - row-{a}-column-lines-y-{b}    -> Aligns item lines (sub rows, only when row has not the "no wrap" class) within,
                                       when there is extra space on the y axis (cross-axis)

  **Col Options:**

    - col-{a}-auto               -> item will take all free space on x axis
    - col-{a}-hidden             -> display: none for certain media queries
    - col-{a}-self-flow-y-{b}    -> defines itself's alignment along the y axis (cross axis)

  **Flexbox browser support:**

    - Chrome 45+
    - Chrome for Android 49+
    - Firefox 43+
    - Safari 9+
    - iOS Safari 8.4+
    - Opera 35+
    - Opera Mini 8+
    - Edge 13+
    - IE 10+ (partial)
    - Android Browser 4.3+


  **Legend:**
  
    - {a} -> any media query suffix
    - {b} -> flow (type) suffix
