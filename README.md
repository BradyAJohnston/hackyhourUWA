# hackyhourUWA

A running log of things we have managed to fix, and resources we have found along the way!
---

### 2020-04-05
Attendants: 8
 - Fixed problems with `{glmnet}` packackage by converting input matrices from character matrices to numeric matrices
   - suggested to move the analysis to tidymodels at some point - support exists https://parsnip.tidymodels.org/reference/glmnet-details.html
 - learnt how to test for vectors being in other vectors in julia using `in()`
   -  `in.(data.column, [vectors])` to create logical vector to subset `data` rows
     -  important to broadcast the `in()` function, and also put the `vectors` in its own array with `[]` to broadcast against
     -  also learned innerjoin(), intersect(), union() to compare and merge two data-frames

 - fixing Julia Versions, after installing a new version of julia
  - `Pkg.add("IJulia"); Pkg.build("IJulia")` this will re-register the new kernal which Jupyter notebooks etc and anything that requires the kernal.
 - Showed cloudstor.aarnet.edu.au to transfer < 1TB of data internationally (upload via webpage, or use curl https://www.solved.tips/aarnet-cloudstor-using-curl-command-line/ )
 - Played around with visualising PC1, PC2, PC3 across RNAseq datasets using ggplot - use facet_wrap(~GROUP) to check how groups look

### 20220329
Attendants: 7
 - turn your `for` loops into `lapply()` instead
 - Install [Rtools for Windows](https://cran.r-project.org/bin/windows/Rtools/rtools40.html) to install `{Rcpp}` and other packages properly on Windows.
 - Wrote a tiny Python script that parses an Ensembl gff3 to pull out functional annotation for mRNAs
 - Discussed modeling of turtle movement - showed the usefulness of tidymodels and the upcoming tidymodels book https://www.tmwr.org/
 - Showed the Profiler in RStudio for long-running code
 - Introduced Julia to people who need to run many computationally-intensive models
