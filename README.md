# Rworkshop
For the [rtidyverse](https://rworkshop.uni.lu) workshop 


### Installation

1. Setup the RStudio environment by cloning the repository

2. Activate [`renv`](https://rstudio.github.io/renv/articles/renv.html) by running `renv::activate()`. You might need to install `renv` by running `install.packages("renv")`.
3. Run `renv::restore()` to install the package with the version. Say `y` to `Do you want to proceed? [y/N]:`

5. The first tutorial (datasauRus) will be guided and demonstrate capacities in the tidyverse which we will explore in the workshop.

6. The other practicals are yours to complete and push to the repository. 

### Assignments

#### Practical01 Datasaurus

The Rmd document is already ready except for the header.


Currently it is the following:

~~~
---
title: "Datasaurus"
author: "Aurelien Ginolhac"
date: "2021-23-11"
---
~~~

Your tasks:

- Replace the author name by yours
- Fix the date for today following the ISO8610 norm: `YYYY-MM-DD`
- Save the file
- Commit the changes
- Push to the github classroom

#### Other practicals

Use the Rmarkdown templates in this repo by:

- Edit the header accordingly with your name
- Fill out the answer in the R chunks (default filled with a comment `# Write your answer here`)
- Knit the Rmd to check if everything works well
- If you use a new package (_i.e_ `palmerpenguis`), update the `renv.lock` with 
    + `renv::snapshot()`, new package are discovered, say `y` to `[yN]`
    + `Git` add the `renv.lock`, along with the completed Rmd
    + `Git` push
