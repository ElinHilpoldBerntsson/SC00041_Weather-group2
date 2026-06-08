
# Weather Data Visualization



## Project overview



This repository contains an R script for visualizing monthly weather data. The script reads weather data from a CSV file and creates a plot showing monthly temperature and precipitation.



The project was completed as part of Assignment 2.2 for Group 2.



## Repository structure



```text

SC00041_Weather-group2/

├── data/

│   └── weather_data.csv

├── environment.yml

├── plot_weather.R

└── README.md

```



## Data



The input data is stored in:



```text

data/weather_data.csv

```



The CSV file contains monthly weather observations with these expected columns:



| Column | Description |

|---|---|

| `Month` | Name of the month |

| `Year` | Year of the observation |

| `Temperature` | Average monthly temperature |

| `Precipitation` | Monthly precipitation |



## Software environment



This project uses a conda environment to make the analysis reproducible.



The environment is defined in:



```text

environment.yml

```



The environment includes:



| Package | Purpose |

|---|---|

| `r-base` | Provides the R programming language |

| `r-ggplot2` | Used to create the weather plot |

| `r-dplyr` | Used for data handling |

| `r-readr` | Used to read the CSV file |



Using `environment.yml` helps make sure that everyone can run the project with the same required software and R packages.



## Creating the conda environment



From the main folder of the repository, run:



```bash

conda env create -f environment.yml

```



This creates a conda environment called:



```text

weathergroup2

```



## Activating the environment



Before running the script, activate the environment:



```bash

conda activate weathergroup2

```



## Checking the environment



Check that R is installed:



```bash

R --version

```



Check that the required R packages are installed:



```bash

Rscript -e "library(ggplot2); library(dplyr); library(readr)"

```



If this runs without errors, the environment is ready.



## Running the script



Make sure you are in the main repository folder, then run:



```bash

Rscript plot_weather.R

```



The script will:



1. load the required R packages;

2. read `data/weather_data.csv`;

3. prepare the month order;

4. create a weather plot;

5. create an `output/` folder if it does not already exist;

6. save the plot as a PNG file.



## Output



The output file is saved as:



```text

output/weather_plot.png

```



The plot shows:



- precipitation as bars;

- average temperature as points and lines;

- separate panels for each year.



## Authors



Nina Gotzmann

Elin Hilpold Berntsson

Ana-Maria Matota
