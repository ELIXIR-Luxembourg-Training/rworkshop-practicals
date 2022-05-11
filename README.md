# Rworkshop

For the [rtidyverse](https://rworkshop.uni.lu) workshop 

### Installation

1. Setup the RStudio environment by cloning the repository

2. Install [`renv`](https://rstudio.github.io/renv/articles/renv.html) and `yaml` by running ``install.packages(c("renv", "yaml"))`

3. Activate `renv` by running `renv::activate()`. 

4. Run `renv::hydrate()` to install the packages necessary. You should see:

```
* Discovering package dependencies ... Done!
* Copying packages into the cache ... Done!
```

Should be fast since you already have most packages in your `renv` cache.

5. Create your first package snapshot() with `renv::snapshot()`. Output is:

```
The following package(s) will be updated in the lockfile:

# CRAN ===============================
- R6           [* -> 2.5.1]
- base64enc    [* -> 0.1-3]
- bslib        [* -> 0.3.1]
[...]
- tinytex      [* -> 0.38]
- xfun         [* -> 0.30]
- yaml         [* -> 2.3.5]

Do you want to proceed? [y/N]: 
```

Say `y` to `Do you want to proceed? [y/N]:`. The `renv.lock` is created.

6. The first tutorial (**datasauRus**) will be guided and demonstrate capacities in the tidyverse which we will explore in the workshop.

7. The other practicals are yours to complete and push to the repository. 

### Assignments

#### Practical01 Datasaurus

The Rmd document is already ready except for the header.


Currently it is the following:

~~~
---
title: "Datasaurus"
author: "Aurelien Ginolhac"
date: "2022-05-12"
---
~~~

Your tasks:

- Replace the author name by yours
- Save the file
- Commit the changes
- Push to the GitHub classroom

#### Other practicals

Use the Rmarkdown templates in this repo by:

- Edit the header accordingly with your name
- Fill out the answer in the R chunks (default filled with a comment `# Write your answer here`)
- Knit the Rmd to check if everything works well
- If you use a new package (_i.e_ `palmerpenguis`), update the `renv.lock` with 
    + `renv::snapshot()`, new package are discovered, say `y` to `[yN]`
    + `Git` add the `renv.lock`, along with the completed Rmd
    + `Git` push
