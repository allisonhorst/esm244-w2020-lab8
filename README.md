# ESM 244 (Winter 2020) - Lab Week 8

### Text mining, sentiment analysis, and visualization

### Resources:

- Julia Silge and David Robinson's [Text Mining with R](https://www.tidytextmining.com/)

### Packages you'll need:

**For text mining & analysis stuff**: 

- `tidyverse`
- `here`
- `pdftools`
- `textdata`
- `tidytext`
- `ggwordcloud`


**Note - before lab for sentiment analysis you will need to:**

- Attach `tidytext` and `textdata` packages
- In the console, Run: `get_sentiments(lexicon = "nrc")`
- You should be prompted to install lexicon - choose yes!
- Once that's done, in the console run `get_sentiments(lexicon = "afinn")`
- You should be prompted to install lexicon - choose yes!

**For point pattern analysis example:**

- `sf`
- `rgdal`
- `spatstat`
- `sp`
- `maptools` version 0.9-5 (we think this was the issue with point pattern analysis we saw last week). 

To get `maptools` v0.9-5, run the following: 

```
detach("package:maptools",unload=TRUE)
library(devtools)
install_version("maptools", version="0.9-5")
```

### Data: 

- IPCC (International Panel on Climate Change) Special Report: Global Warming of 1.5 degrees. 
- Sage grouse telemetry, Mono County:
    - Data summary: CA DFG sage grouse telemetry (Mono County)
    - Files: ds68 layer
    - Contact: William Perry, US Geological Survey (USGS)
    - Link: https://map.dfg.ca.gov/metadata/ds0068.html
