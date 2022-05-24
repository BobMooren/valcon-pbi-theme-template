# Theme Template

Valcon (Sneaker Faqtory) template of Power BI JSON file

## To Do

#### Document  general properties
- [X] Colorscheme
- [X] Text/fonts
- [ ] General
- [ ] Axis
- [ ] Legend
#### Visual specific properties
- [ ] Add & document stacked bar chart
- [ ] Add & document stacked column chart
- [ ] Add & document clustered bar chart
- [ ] Add & document clustered column chart
- [ ] Add & document 100% bar chart
- [ ] Add & document 100% column chart
- [ ] Add & document line chart
- [ ] Add & document area chart
- [ ] Add & document stacked area chart
- [ ] Add & document line and stacked column chart
- [ ] Add & document and clustered column chart
- [ ] Add & document ribbon chart
- [ ] Add & document waterfall chart
- [ ] Add & document funnel chart
- [ ] Add & document scatter chart
- [ ] Add & document circle chart
- [ ] Add & document donut chart
- [ ] Add & document treemap
- [ ] Add & document gauge
- [ ] Add & document card
- [ ] Add & document multirow card
- [ ] Add & document KPI
- [ ] Add & document filter/slicer
- [ ] Add & document table
- [ ] Add & document matric
- [ ] Add & document decomposition tree

## Known issues


In the following table the known issues and bugs are listed:
 
| Visual    | Issue                                  |
|-----------|----------------------------------------|
| KPI       | Callout value display units not working|


## Example

Below, an empty general template is shown:
```json
{
    "name": "ValconSFTemplate",
    "dataColors": [
        "#60BF81",
        "#3B8C66",
        "#93D94E",
        "#347355",
        "#223240",
        "#60BF81",
        "#3B8C66",
        "#93D94E"
    ],
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
    "null": "#FF7F48",
    "textClasses": {
        "callout": {
            "fontSize": 45,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#252423"
        },
        "title": {
            "fontSize": 12,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#252423"
        },
        "header": {
            "fontSize": 12,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#252423"
        },
        "label": {
            "fontSize": 12,
            "fontFace": "Arial",
            "color": "#252423"
            
        },
        "smallLabel": {
            "color": "#E6E6E6"
        }
    },
    "visualStyles": {
        "*": {
            "*": {
                "general": [
                    {
                        "responsive": true,
                        "keepLayerOrder": true
                    }
                ],
                "legend": [
                    {
                        "showTitle": false,
                        "position": "Top",
                        "show": true
                    }
                ],
                "title": [
                    {
                        "show": true,
                        "titleBold": true
                    }
                ],
                "valueAxis": [
                    {
                        "show": true,
                        "position": "Bottom",
                        "showAxisTitle": true,
                        "axisStyle": "showBoth"
                    }
                ],
                "categoryAxis": [
                    {
                        "show": true,
                        "position": "Left",
                        "showAxisTitle": true,
                        "axisStyle": "showBoth"
                    }
                ],
                "labels": [
                    {
                        "show": false
                    }
                ],
                "*": [
                    {
                        "titleWrap": true,
                        "responsive": true,
                        "percentageLabelPrecision": "2",
                        "labelPrecision": "2"
                    }
                ]
            }
        }
    }
}
AANVULLEN
```