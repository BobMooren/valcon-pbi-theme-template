# Documentation of JSON file

The first line `"name: "ValconSFTemplate"` refers to the name of the theme.
The colors, formatted as an array filled with hex codes, can be set with as shown in the following code block:
```json
{
    "dataColors": [
        "#60BF81",
        "#3B8C66",
        "#93D94E",
        "#347355",
        "#223240",
        "#60BF81",
        "#3B8C66",
        "#93D94E"
    ]
}
```
Other color classes that can be set, are shown in the following table:

```json
{
    "firstLevelElements": "#252423",
    "secondLevelElements": "#605E5C",
    "thirdLevelElements": "#8F8F8F",
    "fourthLevelElements": "#B3B0AD",
    "background": "#FFFFFF",
    "secondaryBackground": "#C8C6C4",
    "tableAccent": "#60BF81",
    "good": "#60BF81",
    "neutral": "#D9B300",
    "bad": "#D64554",
    "maximum": "#118DFF",
    "center": "#D9B300",
    "minimum": "#DEEFFF",
    "null": "#FF7F48"
}
```
These are further explained in the following table:
<table aria-label="Setting structural colors" class="table table-sm">
   <thead>
      <tr>
         <th>Color class preferred name</th>
         <th>Also called</th>
         <th>What it formats</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td><strong>firstLevelElements</strong></td>
         <td><strong>foreground</strong></td>
         <td>Labels background color (when outside data points) <br> Trend line color <br>  Textbox default color <br> Table and matrix values and totals font colors Data bars axis color <br> Card data labels <br> Gauge callout value color <br> KPI goal color <br>  KPI text color <br> Slicer item color (when in focus mode)  <br> Slicer dropdown item font color <br> Slicer numeric input font color <br> Slicer header font color <br> Scatter chart ratio line color <br> Line chart forecast line color <br> Map leader line color <br> Filter pane and card text color <br> Modern visual tooltips text and icon color (Preview)</td>
      </tr>
      <tr>
         <td><strong>secondLevelElements</strong></td>
         <td><strong>foregroundNeutralSecondary</strong></td>
         <td>"light" <a href="#setting-formatted-text-defaults" data-linktype="self-bookmark">secondary text classes</a> <br> Label colors  <br> Legend label color <br> Axis label color <br> Table and matrix header font color <br> Gauge target and target leader line color <br>  KPI trend axis color <br> Slicer slider color <br> Slicer item font color <br> Slicer outline color <br> Line chart hover color <br> Multi-row card title color <br> Ribbon chart stroke color <br> Shape map border color <br> Button text font color <br> Button icon line color <br> Button outline color</td>
      </tr>
      <tr>
         <td><strong>thirdLevelElements</strong></td>
         <td><strong>backgroundLight</strong></td>
         <td>Axis gridline color <br> Table and matrix grid color <br> Slicer header background color (when in focus mode)  <br> Multi-row card outline color  <br> Shape fill color <br> Gauge arc background color <br> Applied filter card background color <br> When background = FFFFFF: <br> Disabled button fill color <br> Disabled button outline color <br></td>
      </tr>
      <tr>
         <td><strong>fourthLevelElements</strong></td>
         <td><strong>foregroundNeutralTertiary</strong></td>
         <td>legend dimmed color <br> Card category label color <br> Multi-row card category labels color <br> Mulit-row card bar color <br> Funnel chart conversion rate stroke color <br> Disabled button text font color <br> Disabled button icon line color <br></td>
      </tr>
      <tr>
         <td><strong>background</strong></td>
         <td aria-label="No value"></td>
         <td>Labels background color (when inside data points) <br> Slicer dropdown items background color  <br> Donut chart stroke color <br> Treemap stroke color <br> Combo chart background color <br> Button fill color <br> Filter pane and available  filter card background color <br> Modern visual tooltips background color (Preview)</td>
      </tr>
      <tr>
         <td><strong>secondaryBackground</strong></td>
         <td><strong>backgroundNeutral</strong></td>
         <td>Table and matrix grid outline color <br> Shape map default color <br> Ribbon chart ribbon fill color (when match series option is turned off) <br> When background != FFFFFF: <br> Disabled button fill color <br> Disabled button outline color <br> Modern visual tooltips separator line and hover color (Preview)</td>
      </tr>
      <tr>
         <td><strong>tableAccent</strong></td>
         <td aria-label="No value"></td>
         <td>Overrides table and matrix grid outline color when present</td>
      </tr>
   </tbody>
</table>

Fonts *across the report* are set within the `textClasses: {}` object. These are similar to color classes, but can update size, color and family of the fonts. Up to 12 different text classes can be set, only 4 are necessary, the secondary classes inherit from the above primary class. Furthermure, these classes can be made bold by adding the property `"bold": true`.

<table aria-label="Table 3" class="table table-sm">
   <thead>
      <tr>
         <th>Primary class</th>
         <th>Secondary classes</th>
         <th>JSON class name</th>
         <th>Default settings</th>
         <th>Associated visual objects</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Callout</td>
         <td>N/A</td>
         <td>callout</td>
         <td>DIN <br> #252423 <br> 45pt</td>
         <td>Card data labels <br> KPI indicators</td>
      </tr>
      <tr>
         <td>Header</td>
         <td>N/A</td>
         <td>header</td>
         <td>Segoe UI Semibold <br> #252423 <br> 12pt</td>
         <td>Key influencers headers</td>
      </tr>
      <tr>
         <td>Title</td>
         <td aria-label="No value"></td>
         <td>title</td>
         <td>DIN <br> #252423 <br> 12pt</td>
         <td>Category axis title <br> Value axis title <br> Multi-row card title * <br> Slicer header</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Large title</td>
         <td>largeTitle</td>
         <td>14pt</td>
         <td>Visual title</td>
      </tr>
      <tr>
         <td>Label</td>
         <td aria-label="No value"></td>
         <td>label</td>
         <td>Segoe UI<br>#252423<br>10pt</td>
         <td>Table and matrix column headers <br> Matrix row headers<br>Table and matrix grid<br>Table and matrix values</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Semibold</td>
         <td>semiboldLabel</td>
         <td>Segoe UI Semibold</td>
         <td>Key influencers profile text</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Large</td>
         <td>largeLabel</td>
         <td>12pt</td>
         <td>Multi-row card data labels</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Small</td>
         <td>smallLabel</td>
         <td>9pt</td>
         <td>Reference line labels * <br>Slicer date range labels<br> Slicer numeric input text style<br>Slicer search box<br>Key influencers influencer text</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Light</td>
         <td>lightLabel</td>
         <td>#605E5C</td>
         <td>Legend text<br>Button text<br>Category Axis labels<br>Funnel chart data labels<br>Funnel chart conversion rate labels<br>Gauge target<br>Scatter chart category label<br>Slicer items</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Bold</td>
         <td>boldLabel</td>
         <td>Segoe UI Bold</td>
         <td>Matrix subtotals<br>Matrix grand totals<br>Table totals</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Large and Light</td>
         <td>largeLightLabel</td>
         <td>#605E5C<br>12pt</td>
         <td>Card category labels<br>Gauge labels<br>Multi-row card category labels</td>
      </tr>
      <tr>
         <td>-</td>
         <td>Small and Light</td>
         <td>smallLightLabel</td>
         <td>#605E5C<br>9pt</td>
         <td>Data labels<br>Value axis labels</td>
      </tr>
   </tbody>
</table>

adfadsf