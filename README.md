# Animated Visualizations with ggplot2 and gganimate

This project creates animated visualizations in R using `ggplot2`, `gganimate`, and `sf` libraries. It includes two main parts: a simple bar chart animation and an animated map visualization based on shapefile data. The animations showcase smooth transitions in color to represent changes over time.

## Code Overview

### 1. Toy Example: Bar Chart Animation
   - **Dataset**: A simple dataset with a constant value `x` and a categorical variable `state_cont` representing different states or categories.
   - **Color Transition**: A custom color palette is created with eight colors, applied in a gradient transition across categories.
   - **Animation**: The bar chart shows smooth transitions in color over "time" frames, with each frame moving to the next category.

### 2. Map Visualization with Shapefiles
   - **Shapefile Data**: Loads spatial data for a geographical area (in this case, Barcelona) as polygons.
   - **Categorical Variable**: Each region is colored based on a categorical variable (`random`), with a color palette applied for differentiation.
   - **Rotation**: The map undergoes a slight geometric rotation for visual effect.

### 3. Preparing Data for Map Animation
   - **Time Frames**: The categorical variable `random` is incremented for each time frame in a cyclic manner. This creates a gradual color change in each region across frames.
   - **Combined Data**: All frames are compiled into a single dataset for smooth transition animation.

### 4. Animated Map with Color Transitions
   - **Animation Creation**: The map is animated over time, with each frame representing a different time step. Colors transition smoothly from one frame to the next.
   - **Rendering**: The animation is rendered as an MP4 video file, with settings for frame rate, resolution, and duration.

## Purpose
The project is designed to create visually engaging animations that represent temporal or state-based changes. The animations are suitable for displaying gradual changes in categorical variables, both in simple bar charts and in geographical maps. This approach is useful for presentations or visual storytelling where visualizing transitions over time enhances understanding.

## Prerequisites
- R packages: `ggplot2`, `gganimate`, `sf`, and `colorspace`.
- A compatible shapefile for the map visualization.

## Output
- Bar chart animation: Displays color transitions across different categories.
- Animated map: Shows color transitions across regions in a rotated map.

## Usage
To run the code, simply execute the R script. Adjust the parameters in the animation settings (e.g., duration, frame rate) as needed.


## FIG 1: Toy example. simple square transitioning over a predifined color palette

![alt text](https://github.com/JuanGaleano/gganimate_map_colors/blob/main/toy_example.gif) 
