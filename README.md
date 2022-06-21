# Theme Template

Valcon template of Power BI JSON file

## To Do

- [ ] Define standard template
- [ ] Update documentation 

## Known issues


In the following table the known issues and bugs are listed:
 
| Visual    | Issue                                                                 |
|-----------|-----------------------------------------------------------------------|
| KPI       | Callout value display units not working                                                            
| General   | Precision of data (decimal placement) should also be set in data view 
| Treemap   | Title not bold


## Template

Below, an empty general template, without a background, is shown. For a JSON with a background, check the /json/theme_template.json:
```json
{
    "name": "ValconSFTemplate",
    "dataColors": [
        "#1E64E8",
        "#8fb2f4",
        "#1850ba",
        "#4b83ed",
        "#0f3274",
        "#3F4E69",
        "#06142e",
        "#123c8b"
    ],
    "firstLevelElements": "#262622",
    "secondLevelElements": "#969696",
    "thirdLevelElements": "#E6E6E6",
    "fourthLevelElements": "#969696",
    "background": "#FFFFFF",
    "secondaryBackground": "#E6E6E6",
    "tableAccent": "#1E64E8",
    "good": "#60BF81",
    "neutral": "#D9B300",
    "bad": "#EE5743",
    "textClasses": {
        "callout": {
            "fontSize": 45,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#262622"
        },
        "title": {
            "fontSize": 12,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#262622"
        },
        "header": {
            "fontSize": 12,
            "fontFace": "Arial",
            "bold": true,
            "titleBold": true,
            "color": "#262622"
        },
        "label": {
            "fontSize": 12,
            "fontFace": "Arial",
            "color": "#262622"
            
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
                        "show": false,
                        "labelPrecision": "2",
                        "showSeries": false
                    }
                ],
                "outspacePane": [
                    {
                        "backgroundColor": {
                            "solid": {
                                "color": "#262622"
                            }
                        },
                        "foregroundColor": {
                            "solid": {
                                "color": "#FFFFFF"
                            }
                        },
                        "checkboxAndApplyColor": {
                            "solid": {
                                "color": "#1E64E8"
                            }
                        }
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
        },
        "treemap": {
            "*": {
                "labels": [
                    {
                        "show": true,
                        "color": {
                            "solid": {
                                "color": "#E6E6E6"
                            }
                        }
                    }
                ]
            }
        },
        "textbox": {
            "*": {
                "general": [
                    {
                        "keepLayerOrder": true
                    }
                ],
                "visualHeader": [
                    {
                        "show": false
                    }
                ],
                "background": [
                    {
                        "transparency": 100
                    }
                ]
            }
        }
    }
}
```
