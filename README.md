# Weather Data Visualization

## Purpose
The R script reads a weather csv file and plots data from ths.
The file includes monthly data of the weather and with the script we plot average temperature and precipitatin per month, grouped by year. 
The plot is then saved in the /output directory.

## Instructions for Running Code

### Install dependencies
Make sure you have R installed. The required packages are listed in `environment.txt`. Install them by running the following in R:

```r
install.packages("ggplot2")
install.packages("dplyr")
install.packages("readr")
```

### Run the script
Be in the repository including the R script and the /data directory, and run:

```bash
Rscript plot_weather.R
```

NOTE: Make sure the `data/weather_data.csv` file is present before running the script. 
The script will automatically create the `output/` folder if not created before running it.

## What output to expect
A PNG file named `weather_plot.png` will be saved in the `output/` folder. This plot shows temperature and rain per month, grouped by year.
The precipitation is vizualized as bars with the values stated on the right y-axis. The temperature is shown as points for average temp.,
and a line connecting the points month to month, with values on the left y-axis.
