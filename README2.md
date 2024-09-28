# nice888setup

The goal of nice888setup is to provide a template for an R package project to start off. You will need to finish the rest.

``` r
remotes::install_github('Throwback8491/nice888setup')
```

# Further setup instructions

1.  use_X_license

2.  use_author

4.  find and replace all instances of "nice888setup" and replace them with the title of the package you actually want to make

5.  run the commented out renv::install commands

7.  rename the Rproj file to the same thing as step 4

8.  delete the git repo

9.  reopen rstudio

11. use_git()

add the following snippet (but better formatted). my_sinew_force will be a living list that keeps growing as I discover annoying sinew namespacing defaults

snippet nss	usethis::use_r("\${1}")	sinew::pretty_namespace("R/\${1}.R", force = my_sinew_force, overwrite = TRUE)	file.remove("R/\${1}.R")
