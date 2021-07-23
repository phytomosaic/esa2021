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


This is a dedicated R package that contains tutorial material.  Install using _either_ method 1 _or_ method 2.

### Installation method 1

This method should be most simple.

1.  Download and install R from CRAN: https://cran.r-project.org/.
<!-- 2.  If you are on a Windows platform, download and install Rtools from https://cran.r-project.org/bin/windows/Rtools/ -->
2.  Download the package from:  https://github.com/phytomosaic/taresa2021/raw/main/esa2021_0.0.1-20210722.tar.gz and save somewhere you will remember.
3.  Open the R console and run:

```
### install dependencies
pkg <- c('vegan','labdsv','ade4','ecodist','fso',
         'vegclust','ape','picante','mgcv','learnr')
has <- pkg %in% rownames(installed.packages())
if(any(!has)) install.packages(pkg[!has])

### specify path to wherever you saved the file (change as needed)
path_to_file <- '~/Downloads/esa2021_0.0.1-20210722.tar.gz'

### install the main package
install.packages(path_to_file, repos=NULL, type='source')
```
4. Go to **Usage** below.

### Installation method 2

Use this method if build tools are already installed on your system (if you don't know what build tools are, then use method 1 above).

1.  Download and install R from CRAN: https://cran.r-project.org/.
<!-- 2.  If you are on a Windows platform, download and install Rtools from https://cran.r-project.org/bin/windows/Rtools/ -->
2.  Open the R console and run the following (agree to update any packages, and you may need to repeat if the first download attempt was unsuccessful):

```
install.packages('remotes')
require(remotes)
remotes::install_github('phytomosaic/esa2021')
```
3. Go to **Usage** below.

### Usage

To run the tutorial, simply run this in the R console:
  
```
require('esa2021')
learnr::run_tutorial('esa_tutorial', package='esa2021')
```

This creates a local instance of the interactive tutorial, which can open in a web browser.  The tutorial is a combination of text describing ecological concepts, along with embedded code chunks that let you run live R commands.

### Pre-survey

Don't forget to fill out the survey _before_ the course.  This lets us know which topics you'd like to focus on.  Find it at: https://www.surveymonkey.com/r/K9C9QKP


### Contributors

**Organizer**: Kyle Palmquist  
**Co-organizers**: Martin Dovciak, Samuel Jordan, Lisa Kluesner, Rob Smith (robert.smith3@usda.gov)  
