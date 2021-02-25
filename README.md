# esa2021

ESA 2021 workshop: community analysis of species, traits, phylogenies, and responses to environment


### Session principles
- broad-and-shallow topic coverage  
- use base R and other FOSS (free and open-source software)  
- require minimal dependencies  


### Session audience
- Researchers and academics  
- Forest and grassland managers  
- Computational ecologists  
- Students and early-career vegetation ecologists  


### Installation

1. Download and install R from CRAN: https://cran.r-project.org/.
2. Download and install the `esa2021` package: `remotes::github_install('phytomosaic/esa2021')`.
3. Install the `learnr` package: `install.packages('learnr')`.
4. Follow instructions below.


### Usage

To run the tutorial, simply run this in the R console:

```
require('esa2021')
require('learnr')
learnr::run_tutorial('esa_tutorial', package = 'esa2021')
```

This creates a local instance of the interactive tutorial.  The tutorial is a combination of text describing ecological concepts, along with embedded code chunks that let you run live R commands.

### Contributors

**Organizer**: Kyle Palmquist  
**Co-organizers**: Martin Dovciak, Samuel Jordan, Lisa Kluesner, Rob Smith (robert.smith3@usda.gov)  

