# Key Terms

### Visualization packages for R:

- ggplot2
- Plotly
- Lattice
- RGL
- Dygraphs
- Leaflet
- Highcharter
- Patchwork
- gganimate
- ggridges

## ggplot2 - most popular visualization package in R

- Benefits of ggplot2:
  - Create different types of plots
  - Customize the look and feel of plots
  - Create high quality visuals
  - Combine data manipulation and visualization
- Core concept of ggplot2:
  - Aesthetics
  - Geoms
  - Facets
  - Labels and annotations
- Using ggplot2:
  1. Start with the ggplot function and choose a dataset to work with
  2. Add `+` a geom\_ function to display your data
     - plus sign to add a layer to your plot
  3. Map the variables you want to plot in the arguments of the aes() function

### Aesthetic - A visual property of an object in your plot

- `aes()`: selecting the feature to use
- `x=`: x-axis
- `y=`: y-axis
- `color=`: color coding, color border
- `fill=`: color inside
- `shape=`: different shape
- `size=`: different size
- `alpha=`: transparence

### Geom - The geometric object used to represent your data

- `geom_point()`: using points or scatter chart
- `geom_bar()`: bar chart
- `geom_line()`: line chart
- `geom_smooth()`: show trend
- `geom_jitter()`: scatter chart with added small amount of random noise to each point in the plot
- `mapping=`: attrubite for matching the aesthetic of the plot

### Facets - Let you display smaller groups, or subsets, of your data

- `facet_warp()`: adding multiplot, using `~` in front of features
- `facet_grid()`: split graph vertically by first variable, horizontally by second variable

### Labels and annotations - Let you customize your plot

- The benefits of adding annotations:
  - Indicating the main purpose
  - Highlighting important data
  - Helping stakeholders quickly understand your plot
- `labs()`: label function
- `title=`: add title to plot, display at top
- `subtitle=`: add subtitle to plot, display below title
- `caption=`: add caption, display at bottom right

### Annotate - To add notes to a document or diagram to explain or comment upon it

- `annotate()`: display information

### Mapping - matching up a specific variable in your dataset with a specific aesthetic

### Saving your visualizations:

- Export option in Rstudio
- `ggsave()`
