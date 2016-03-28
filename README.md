# css3-flexbox-grid
A lightweight grid system based on CSS3 Flexbox

Flexbox is a new layout mode in CSS3, it consists of flex containers and flex items.

The grid system uses similar syntax than bootstrap to make it easy to switch.


  **Versions:**
    
    - flexbox-grid.css -> 12 Units per row, Media Queries 500, 750, 1000
    - flexbox-grid.min.css -> same as flexbox-grid.css but compressed
    - flexbox-grid-24units.css -> 24 Units per row, Media Queries 500, 750, 1000    
    - flexbox-grid-24units.min.css -> same as flexbox-grid-24units.css but compressed    


  **Example:**

    ![alt text](https://github.com/tobiasvitt/css3-flexbox-grid/example/img/flex-items-width.png "Flex Items Width")
    ```
                <div class="col-12 row">
                    <div class="col-1">Size 1 / col-1</div>
                </div>
                <div class="col-12 row">
                    <div class="col-2">Size 2 / col-2</div>
                </div>
                <div class="col-12 row">
                    <div class="col-3">Size 3 / col-3</div>
                </div>
                <div class="col-12 row">
                    <div class="col-4">Size 4 / col-4</div>
                </div>
                <div class="col-12 row">
                    <div class="col-5">Size 5 / col-5</div>
                </div>
                <div class="col-12 row">
                    <div class="col-6">Size 6 / col-6</div>
                </div>
                <div class="col-12 row">
                    <div class="col-7">Size 7 / col-7</div>
                </div>
                <div class="col-12 row">
                    <div class="col-8">Size 8 / col-8</div>
                </div>
                <div class="col-12 row">
                    <div class="col-9">Size 9 / col-9</div>
                </div>
                <div class="col-12 row">
                    <div class="col-10">Size 10 / col-10</div>
                </div>
                <div class="col-12 row">
                    <div class="col-11">Size 11 / col-11</div>
                </div>
                <div class="col-12 row">
                    <div class="col-12">Size 12 / col-12</div>
                </div>

    ```
    ![alt text](https://github.com/tobiasvitt/css3-flexbox-grid/example/img/flex-items-x-flow.png "Flex Items Flow X-Axis")

    ![alt text](https://github.com/tobiasvitt/css3-flexbox-grid/example/img/flex-items-y-flow.png "Flex Items Flow Y-Axis")

    ![alt text](https://github.com/tobiasvitt/css3-flexbox-grid/example/img/flex-items-column-lines-positions.png "Flex Items Column lines position")

    ![alt text](https://github.com/tobiasvitt/css3-flexbox-grid/example/img/flex-items-self-alignment.png "Flex Items Self Alignment")


  **Media Queries:**
     
    - col-{b}      -> grid columns independent from media query
    - col-xs-{b}   -> "extra small" 0px - 500px 
    - col-sm-{b}   -> "small"       500px - 750px
    - col-md-{b}   -> "medium"      750px - 1000px
    - col-lg-{b}   -> "large"       1000px - unlimited


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


  **Flexbox Browser Support:**

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


   **Configure SCSS Version:**
   
    1. Constants:
   
      - $browser-context      -> Defines the default pixel size
      - $row-max-width        -> Defines the number of units a grid row can contain
      - $col-{a}-breakpoint   -> Defines the breakpoint for a specific media query
   
    2. Media queries:
   
      - col-{b}      -> grid columns independent from media query
      - col-xs-{b}   -> 0px - $col-xs-breakpoint
      - col-sm-{b}   -> $col-xs-breakpoint - $col-sm-breakpoint
      - col-md-{b}   -> $col-sm-breakpoint - $col-md-breakpoint
      - col-lg-{b}   -> $col-md-breakpoint - unlimited


  **Legend:**
  
    - {a} -> any media query suffix
    - {b} -> flow (type) suffix
