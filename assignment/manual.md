# What is LocusZoom (Ford)
PLZ DO NOT COPY THE CONTENT IN THE WEBSITE TO ANSWER HERE!!!!! PARAPHRASE IT!!!

# Getting Started (Ford)
Explanation of components in the website, what it can do?, What are the different of 4 modes? (Single Plot with your own data, single plot with published GWAS Data, Batch Plot with HITSPEC and Interactive plot with published GWAS)

# How to analyse (Nung)

# How to Interpret the Result (Beer)
Plot published GWAS has two mode include single plot and interactive plot
**1. Single plot**
- Choose Pre-loaded data type by selecting trait group and data file.
- Specify region to display by fill in only of SNP reference name, Gene reference name, or region
- Use option controls to add more specific details such as Genome Build/LD Population for choosing reference genome from population
- Click Plot data. PDF file's downloaded to computer.

**2. Interactive plot** 
- Use the + ADD STUDY and + ADD BED TRACK buttons to add other published GWAS results and published annotation (BED) tracks.
- Use the X button whicch appears when cursor is on the plot to remove data.
- Explore different regions in the genome in a variety of different ways:
    - Click and drag the plot to pan left/right
    - Shift+Scroll the mousewheel to zoom in or out
    - Click and drag x-axis or y-axis ticks to scale that axis
    - Shift+click and drag x-axis or y-axis ticks to pan along that axis
    - Use the Pan / Zoom Region buttons to navigate around the currently shown region
    - Use the Show Region By Gene dropdown to jump to regions centered around preselected genes
    - Go to specific region by enter the format chr:start-end
- Click on genes or variants in any part of the plot for more information about them
- Use the up and down  buttons to swap the plot up and down
- Use the Abstract button to see more information about the data that panel is showing
- Click and drag the bars between panels to resize them
- Use the Download Image button to export an SVG image of the plot, suitable for converting to PDF or any other image format

***Features and functionality***
![](./img/hdl interactive.png)
Fig. 1. An example LocusZoom plot showing the HDL cholesterol-associated region near the MCM6 gene from interactive mode

![](./img/hdl single1.png)
![](./img/hdl single2.png)
Fig. 2. An example LocusZoom plot showing the HDL cholesterol-associated region near the MCM6 gene from single mode and details.

- The main panel of a LocusZoom plot shows association P-values on the -log10 scale on the vertical axis, and the chromosomal position along the horizontal axis.
- The user can specify the region to display in one of three ways: 
  1. an index SNP and a window size
  2. the chromosome together with start and stop positions
  3. gene name and size of flanking region. 
- The plots were designed to display ~1 Mb windows of the genome, although for regions with several association signals or long-range LD patterns, plots extending further can be drawn.
- To identify SNPs that may be potentially causative, LocusZoom plots show not only the magnitude of association for each SNP, but also the pairwise LD pattern with the most strongly associated SNP or another user-specified SNP. 
- Quick inspection can reveal the extent of the associated region and the location and number of SNPs in strong LD with the index SNP. In addition, a locus may show strongly associated variants that are weakly correlated, suggesting the presence of multiple independent association signals.
- Users may choose to display LD (r^2). LocusZoom is compatible with 1000 Genomes SNP naming format (chr:position) and will plot association results for novel SNPs identified by sequencing studies.
- The bottom panel of a LocusZoom plot shows the name and location of genes. Positions of exons are displayed, and the transcribed strand is indicated with an arrow. This allows the visual comparison of association results relative to coding regions. Gene names are automatically spaced relative to one another to avoid overlap.
- The details from graph including:
  - date: show date and time that interprete the graph
  - buld: reference genome (ie. hg19 is human genome)
  - hilite range
  - reference SNP: chromosome:SNP's positon (ie. chr2:136608646)
  - number of SNPs plotted
  - min P.value
  - max P.value
 Smaller p value means more power of the association effect between variant on metabolic traits.

