GEO 712 Repository
================

# About This Repository

This repository was created for [GEOG
712](https://github.com/paezha/Reproducible-Research-Workflow/tree/master).
It contains activities completed for the course, including examples of
Markdown and information about my research interests.

## Repository Folder Structure

- **data/**: Contains data used in the activities.
- **easter-egg/**: Contains an easter egg.
- **renv/**: Contains files used by the `renv` package to manage the R
  project environment and support reproducibility.
- **README.Rmd**: The main R Markdown file.
- **README.md**: The rendered Markdown file generated from README.Rmd
  and displayed on GitHub.
- **renv.lock**: Records the R package dependencies and versions used in
  the project.

# About Me

## Academic Achievements

BSc Environmental Science - McMaster University (2022-2026)

MSc Earth and Environmental Science - McMaster University (2026-Present)

# Research Interest

My research interest is **tree-level biomass estimation** using [*remote
sensing*](https://en.wikipedia.org/wiki/Remote_sensing). I am interested
in using LiDAR, RGB imagery, and machine learning to estimate the
biomass of individual urban trees.

# Favourites

## Favourite Music

1.  Every Teardrop Is a Waterfall - Coldplay
2.  Liberian Girl - Michael Jackson
3.  Across the Universe - The Beatles
4.  Welcome to Paradise - Green Day
5.  Godlight - Noah Kahan

## Favourite Equation

$$
a^2+b^2=c^2
$$

## Favourite Artists

| Name | Achievements |
|----|----|
| The Beatles | The best-selling artists of all time, with 19 No. 1 albums |
| Michael Jackson | His album “Thriller” is the best-selling album of all time |
| Coldplay | One of the world’s most successful modern rock bands |
| Beabadoobee | Her album “This Is How Tomorrow Moves” reached No. 1 on the UK Albums Chart |
| Frank Sinatra | One of the most celebrated vocalists of the 20th century |

# A Chunk of Code

``` r
print("Hello, World")
```

    ## [1] "Hello, World"

# Hamilton Tree Inventory: Spatially Matched 2018 and 2025 Records

``` r
my_data <- read.csv("data/hamilton_trees_2018_2025_final.csv")

knitr::kable(head(my_data),
             caption = "Hamilton Tree Inventory: Spatially matched tree records from the 2018 and 2025 municipal inventories.")
```

| SPECIES | COMMON.NAM | DBH | X | Y | X2018_SPECI | X2018_COMMO | X2018_DBH | Sci_2025_clean | Sci_2018_clean | Species_Match | DBH_change | IQR_Flag | annual_dbh_change |
|:---|:---|---:|---:|---:|:---|:---|---:|:---|:---|---:|---:|:---|---:|
| Liriodendron tulipifera | Tuliptree | 14 | 597095.1 | 4780967 | Liriodendron tulipifera | TULIP_TREE | 10 | liriodendron tulipifera | liriodendron tulipifera | 1 | 4 | keep | 0.5714286 |
| Gymnocladus dioicus | Kentucky Coffeetree | 24 | 589197.9 | 4791364 | Gymnocladus dioicus | KENTUCKY_COFFEE_TREE | 10 | gymnocladus dioicus | gymnocladus dioicus | 1 | 14 | keep | 2.0000000 |
| Juglans nigra | Black Walnut | 36 | 590941.2 | 4785292 | Juglans nigra | BLACK_WALNUT | 29 | juglans nigra | juglans nigra | 1 | 7 | keep | 1.0000000 |
| Acer saccharum | Sugar Maple | 49 | 588783.9 | 4781403 | Acer saccharum | SUGAR_MAPLE | 43 | acer saccharum | acer saccharum | 1 | 6 | keep | 0.8571429 |
| Acer platanoides | Norway Maple | 41 | 596216.3 | 4788024 | Acer platanoides | NORWAY_MAPLE | 30 | acer platanoides | acer platanoides | 1 | 11 | keep | 1.5714286 |
| Acer platanoides | Norway Maple | 59 | 596213.5 | 4788013 | Acer platanoides | NORWAY_MAPLE | 51 | acer platanoides | acer platanoides | 1 | 8 | keep | 1.1428571 |

Hamilton Tree Inventory: Spatially matched tree records from the 2018
and 2025 municipal inventories.
