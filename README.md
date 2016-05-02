# Attitudes towards outreach in particle physics

Presentation prepared for [my talk at PCST 2016](http://pcst.co/conferences/session/2016-04-26/292), showing early results from my PhD research. The presentation itself can be found at https://via.hypothes.is/https://raoofphysics.github.io/201604_PCST

The slides should also be available on a mobile browser, although Firefox isn't loading the interactive plots for some reason. Against my better judgement, I recommend you use Chrome on Android to view the content.

If you use hypothes.is, please annotate the presentation! I will be grateful for any notes you leave.

## Build information

This presentation is put together using:

- [R](https://www.r-project.org/), using [RStudio](https://www.rstudio.com/)
- [ggplot2](http://ggplot2.org/) + [plotly](https://plot.ly/) for the bar plots
- [RAW](http://raw.densitydesign.org/) for the *alluvial* plots
- [knitr](https://cran.r-project.org/web/packages/knitr/index.html) (available within RStudio) + [reveal.js](http://lab.hakim.se/reveal-js/) for the presentation itself
- [hypothes.is](https://hypothes.is/), which provides the annotation layer on top of the presentation

knitr takes the `.Rmd` (R Markdown) file and through some wizardry produces a standalone `.html` file that serves as the presentation.

Please note that efforts to take the `index.Rmd` and build `index.html` **will fail**, since I cannot make the underlying research data public yet. In particular, when the following line is called in the code, the file it refers to (`final_dataset.csv`) can only be found in my private storage space on CERN's internal servers:

```{r}
dat <- read.csv(file = "../quant_analysis/final_dataset.csv", header = TRUE)
```

## Licence

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">Attitudes towards outreach in particle physics</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/RaoOfPhysics/201604_PCST" property="cc:attributionName" rel="cc:attributionURL">Achintya Rao</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

## Acknowledgements

This presentation is part of [my PhD research](http://achintyarao.in/phd), which is supported by the [CMS Collaboration](http://cms.web.cern.ch) at [CERN](http://home.cern) under the CERN Doctoral Student Programme.

I would like to thank my supervisors for guiding me on this project:

- Dr. Emma Weitkamp (UWE), Director of Studies
- Dr. Clare Wilkinson (UWE)
- Dr. Erik Stengler (UWE)
- Dr. Christine Sutton (CERN)

I would also like to thank Richard Smith-Unna ([@blahah404](https://github.com/blahah404)) for his invaluable help with R.
