# Grid system

### How it works <a id="Gridsystem-Howitworks"></a>

Our grid system uses a series of containers, rows, and columns to layout and align content. It’s built with flexbox and is fully responsive. Below is an example and an in-depth look at how the grid comes together.

![](../../.gitbook/assets/screenshot-2017-11-17-grid-system-2.png)

The above example creates three equal-width columns on small, medium, large, and extra large devices using our predefined grid classes. Those columns are centered in the page with the parent `.container`.

Breaking it down, here’s how it works:

* Containers provide a means to center your site’s contents. Use `.container` for fixed width or `.section` for full width.
* Rows are horizontal groups of columns that ensure your columns are lined up properly. We use the negative margin method on `.row` to ensure all your content is aligned properly down the left side.
* Content should be placed within columns, and only columns may be immediate children of rows.
* Column classes indicate the number of columns you’d like to use out of the possible 12 per row. So, if you want three equal-width columns, you can use `.col-xs-4`.
* Column `width`s are set in percentages, so they’re always fluid and sized relative to their parent element.
* There are seven grid tiers, one for each responsive breakpoint: all breakpoints \(extra small\), small, medium, large, and thee extra large sizes \(full hd, 2K, 4K\).

### Grid options <a id="Gridsystem-Gridoptions"></a>

We are using pixels for grid breakpoints and container widths. This is because the viewport width is in pixels and does not change with the font size.

See how aspects of the UI grid system work across multiple devices with a handy table. Gap between 1280 and 1920 - is a 'default' desktop size.



|  | extra small | small | medium | large | extra large | wide screens | 4K |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Container width** | &lt;576px | &lt;768px | &lt;1024px | &lt;1280px | &gt;1920px | &gt;2560px | &gt;3840px |
| **Class prefix** | `.col-xs-` | `.col-s-` | `.col-m-` | `.col-l-` | `.col-xl-` | `.col-xxl-` | `.col-xxxl-` |

