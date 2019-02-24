# What is LocusZoom (Ford)
PLZ DO NOT COPY THE CONTENT IN THE WEBSITE TO ANSWER HERE!!!!! PARAPHRASE IT!!!

# Getting Started (Ford)
Explanation of components in the website, what it can do?, What are the different of 4 modes? (Single Plot with your own data, single plot with published GWAS Data, Batch Plot with HITSPEC and Interactive plot with published GWAS)

# Quickstart
This will show you how to get started using LocusZoom to visualise the GWAS data within web browser.

## LocusZoom Structure

### Plot

 Plot is the main option in LocusZoom, using by the `populate()` method. A plot has a layout and various supported methods.

### Panel

Panel is a subdivided area of a plot which contain graph features for example titles and axes. 

### Data Layer

Data Layer is a layer within a panel for representing data. 

### Dashboard

Dashboard is an HTML element which contain information and user interface components relevant to a plot. Dashboards can be use to attach the plot as a whole or to individual panels. 

### Legend

Legend is an SVG element in panel which present the categories of data shown on the underlying data layers. 

### Making a LocusZoom Plot

#### 1. Include Necessary JavaScript and CSS

the LocusZoom plugin found in the `dist` directory:
* `locuszoom.vendor.min.js` 
This file contains the concatenated vendor libraries. so long as they are included **before including LocusZoom files**.  

* `locuszoom.app.js` OR `locuszoom.app.min.js`  
This is the primary application logic. It should only be included *after* the vendor dependencies have been included.  

* `locuszoom.css`  
This is the primary stylesheet. It is namespaced so as not to conflict with any other styles defined on the same page.

#### 2. Define Data Sources

**Data Sources** is an object representing a collection of arbitrarily many sources from data for the plot. When adding sources to the collection must namespaced so that retrieving specific fields can be done with respect to specific data sources.

for example of defining a data sources object for a remote API by adds an "AssociationLZ" data source (a predefined data source ) with a defined URL. The namespace for this data source as "trait":

```javascript
var data_sources = new LocusZoom.DataSources();
data_sources.add("trait", ["AssociationLZ", { url: "http://server.com/api/" }]);
```

another example:

```javascript
data_sources = new LocusZoom.DataSources();
data_sources.add("trait", ["AssociationLZ", { url: "file:///path/to/data.json" }]);
```

#### 3. Define a Layout

**Layout** is a serializable object that describes the configuration of the LocusZoom plot, including what data will be
pulled from the data sources, displayed in what way, and visual characteristics as color and geometry.

A layout definition example defines a basic plot that is 500 pixels on a side and has one panel with one scatter plot data layer that pulls in position and p-value from the "trait" data source, mapping position to the x axis and pvalue to the y axis:

```javascript
var layout = {
width: 500,
height: 500,
panels: [
{
id: "association",
data_layers: [
{
id: "association",
type: "scatter",
fields: ["trait:position", "trait:pvalue"],
x_axis: { field: "trait:position" },
y_axis: { field: "trait:pvalue" }
}
]
}
]
};
```

#### 4. Wrap up by `LocusZoom.populate()`
 `LocusZoom.populate()` accept a CSS selector  string to populate the first matching element with a plot included, data sources defined, and a layout defined,

example:

```html
<html>
<head>
<script src="locuszoom.vendor.min.js" type="text/javascript"></script>
<script src="locuszoom.app.js" type="text/javascript"></script>
<link rel="stylesheet" type="text/css" href="locuszoom.css"/>
</head>
<body>
<div id="plot"></div>
<script type="text/javascript">
var data_sources = new LocusZoom.DataSources();
data_sources.add("trait", ["AssociationLZ", { url: "http://server.com/api/single/" }]);
var layout = {
width: 500,
height: 500,
panels: [
{
id : "association",
data_layers: [
{
id: "association",
type: "scatter",
fields: ["trait:position", "trait:pvalue"],
x_axis: { field: "trait:position" },
y_axis: { field: "trait:pvalue" }
}
]
}
]
};
var plot = LocusZoom.populate("#plot", data_sources, layout);
</script>
</body>
</html>
```
## Choosing Analysis Mode

![](./img/LocusZoom_Modes.png)

LocusZoom provides 4 modes for visualising GWAS data. In this step, you need to choose the mode of analysis including Single Plot with your owned data, single plot with published GWAS data, batch plot with HITSPEC and interactive plot with published GWAS data. It depends on the data you want to use. If you want to use the published data, you can choose whether single and interactive plot. Otherwise, use your owned data by choosing a single plot with your owned data or batch plot with Hispec.

The difference between the single plot with published GWAS data and the interactive plot is the output from the program. Single plot returns an analysis result as a PDF file which is suitable for making a report while an interactive plot shows the result in the webpage and allows you to investigate the data in more detail.

## Selecting Dataset

![](./img/LocusZoom_Selecting_GWAS.png)

In this example, we focus on using the interactive plot. After select `Interactive Plot`, this page will show up. You may begin by searching for an interested dataset in the search bar. Next, you might navigate through the result from pagination. If the interested dataset has been found, you may click at 'ADD TO PLOT'. The result will appear on top of the webpage.

![](./img/LocusZoom_Single_Owned_Data_Input.png)

If you choose to upload your GWAS data, there is a form for upload and place for fill in the configuration of the visualisation. After filling in the data, you may click at `Plot Your Data` button to get the visualisation of your data.

# How to Interpret the Result (Beer)
