---
name: IS 445 Homework 5 Jekyll Webpage - Bigfoot Sightings Visualizations
tools: [Altair, Python, Vega-Lite]
image: assets/pngs/bigfoot.png
permalink: /projects/IS_445_Homework_5/index.html
description: Interactive visualizations of Bigfoot sightings using Altair & Vega-Lite!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# IS 445 Homework 5 Jekyll Webpage - Bigfoot Sightings Visualizations

This Homework showcases 2 visualizations of Bigfoot sighting data from the [`bfro_reports_fall2022.csv`](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv) dataset, created using Altair, Python, & Vega-Lite. The 1st is a bar chart of sightings by state, & the 2nd is an interactive area chart showing temperature trends over time with a linked overview & detail view. These are exported as JSON files & embedded here for display on this Jekyll webpage.

## Visualization 1: Bar Chart of Bigfoot Sightings by State

<vegachart schema-url = "{{ site.baseurl }}/assets/json/bar_chart.json" style = "width: 100%"></vegachart>

This visualization displays the number of Bigfoot sightings reported across different states, highlighting the geographic distribution of these events. I used a bar chart with the x-axis encoding state names (Nominal data) & the y-axis encoding the count of sightings (Quantitative data). The bars are colored by state using a Tableau20 color scheme to differentiate them visually, though I omitted the legend due to the large number of states for clarity. The x-axis is sorted by count in descending order to emphasize states with the most sightings. On the analysis side, I transformed the data in Python by counting occurrences per state with `value_counts()` & restructuring it into a DataFrame suitable for Altair. There’s no overlap with Homework 6, as this Homework uses a different dataset (`bfro_reports_fall2022.csv`) than Homework 6 ([`building_inventory.csv`](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv)).

## Visualization 2: Interactive Area Chart of Temperature Over Time

<vegachart schema-url = "{{ site.baseurl }}/assets/json/area_chart.json" style = "width: 100%"></vegachart>

This area chart visualizes the mid-temperature of Bigfoot sightings over time, with an upper detailed view & a lower overview chart. The x-axis encodes the sighting date (Temporal data), & the y-axis encodes temperature (Quantitative data), using an area mark to show trends. I added color encoding for season with a Set3 scheme to highlight seasonal variations within the temperature data, ensuring visual distinction. In Python, I transformed the data by converting the `date` column to timestamps with `to_datetime` & filtered out rows with missing date or temperature values for accuracy. For notebook display, a sampled subset (500 rows) was used to keep the file size under 5 MB. This plot differs from Homework 6, which used a scatter plot & the `building_inventory.csv` dataset.

### Interactivity

For the area chart, I implemented an interval selection (`brush`) on the x-axis of the lower overview chart, allowing users to drag a range dynamically updating the upper chart to zoom into the selected time period. This interactivity clarifies temporal trends by enabling exploration of specific date ranges, making it easier to identify patterns in temperature & seasonality, enhancing the visualization’s depth & engagement.

## Search The Data & Methods

Below are links to the dataset & the Python notebook used to generate these visualizations (Note: GitHub doesn't display the plots in the `Workbook.ipynb` file, but `nbviewer` does [here](https://nbviewer.org/github/TheWongLife1/TheWongLife1.github.io/blob/main/python_notebooks/Workbook.ipynb)).

<div class = "left"> {% include elements/button.html link = "https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text = "The Data" %} </div> 

<div class = "right"> {% include elements/button.html link = "https://github.com/TheWongLife1/TheWongLife1.github.io/blob/main/python_notebooks/Workbook.ipynb" text = "The Code" %} </div> 