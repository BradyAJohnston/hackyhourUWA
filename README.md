# hackyhourUWA

A running log of things we have managed to fix, and resources we have found along the way!
---

### 2020-04-05

 - Fixed problems with `{glmnet}` packackage by converting input matrices from character matrices to numeric matrices
 - learnt how to test for vectors being in other vectors in julia using `in()`
   -  `in.(data.column, [vectors])` to create logical vector to subset `data` rows
     -  important to broadcast the `in()` function, and also put the `vectors` in its own array with `[]` to broadcast against

 - fixing Julia Versions, after installing a new version of julia
  - `Pkg.add("IJulia"); Pkg.build("IJulia")` this will re-register the new kernal which Jupyter notebooks etc and anything that requires the kernal.

### 20220329
Attendants: 7
 - turn your `for` loops into `lapply()` instead
 - Install [Rtools for Windows](https://cran.r-project.org/bin/windows/Rtools/rtools40.html) to install `{Rcpp}` and other packages properly on Windows.
 - Wrote a tiny Python script that parses an Ensembl gff3 to pull out functional annotation for mRNAs
 - Discussed modeling of turtle movement - showed the usefulness of tidymodels and the upcoming tidymodels book https://www.tmwr.org/
 - Showed the Profiler in RStudio for long-running code
 - Introduced Julia to people who need to run many computationally-intensive models
