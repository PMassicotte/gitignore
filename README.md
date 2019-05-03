
<!-- README.md is generated from README.Rmd. Please edit that file -->

# gitignore

<!-- badges: start -->

<!-- badges: end -->

The goal of gitignore is to …

## Installation

You can install the released version of gitignore from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("gitignore")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
# devtools::install_github("pmassicotte/gitignore")
library(gitignore)

head(gitignore_fetch_available_templates(), 25)
#>  [1] "1c"                   "1c-bitrix"            "a-frame"             
#>  [4] "actionscript"         "ada"                  "adobe"               
#>  [7] "advancedinstaller"    "agda"                 "al"                  
#> [10] "alteraquartusii"      "altium"               "android"             
#> [13] "androidstudio"        "angular"              "anjuta"              
#> [16] "ansible"              "apachecordova"        "apachehadoop"        
#> [19] "appbuilder"           "appceleratortitanium" "appcode"             
#> [22] "appcode+all"          "appcode+iml"          "appengine"           
#> [25] "aptanastudio"
```

Templates can be fecthed using the `gitignore_fetch_ignore()` function.

``` r
gitignore_fetch_ignore("R")

# Created by https://www.gitignore.io/api/r
# Edit at https://www.gitignore.io/?templates=r

### R ###
# History files
.Rhistory
.Rapp.history

# Session Data files
.RData

# User-specific files
.Ruserdata

# Example code in package build process
*-Ex.R

# Output files from R CMD build
/*.tar.gz

# Output files from R CMD check
/*.Rcheck/

# RStudio files
.Rproj.user/

# produced vignettes
vignettes/*.html
vignettes/*.pdf

# OAuth2 token, see https://github.com/hadley/httr/releases/tag/v0.3
.httr-oauth

# knitr and R markdown default cache directories
/*_cache/
/cache/

# Temporary files created by R markdown
*.utf8.md
*.knit.md

### R.Bookdown Stack ###
# R package: bookdown caching files
/*_files/

# End of https://www.gitignore.io/api/r
```

Multiple templates can be fetched by specifying multiple values:

``` r
gitignore_fetch_ignore(c("java", "c++"))

# Created by https://www.gitignore.io/api/java,c++
# Edit at https://www.gitignore.io/?templates=java,c++

### C++ ###
# Prerequisites
*.d

# Compiled Object files
*.slo
*.lo
*.o
*.obj

# Precompiled Headers
*.gch
*.pch

# Compiled Dynamic libraries
*.so
*.dylib
*.dll

# Fortran module files
*.mod
*.smod

# Compiled Static libraries
*.lai
*.la
*.a
*.lib

# Executables
*.exe
*.out
*.app

### Java ###
# Compiled class file
*.class

# Log file
*.log

# BlueJ files
*.ctxt

# Mobile Tools for Java (J2ME)
.mtj.tmp/

# Package Files #
*.jar
*.war
*.nar
*.ear
*.zip
*.tar.gz
*.rar

# virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
hs_err_pid*

# End of https://www.gitignore.io/api/java,c++
```
