# Checklist of non-native birds in Belgium

## Rationale

This repository contains the functionality to standardize the [Checklist of alien birds in Belgium](https://docs.google.com/spreadsheets/d/1ugsmAq_tlUjFmZef2zyw-mT0Tq1jSdPlNO4KTfJyXVo/edit?usp=sharing) --> to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org).

## Workflow

[source data](data/raw) → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource.do?r=alien-birds-checklist)
* [Dataset on GBIF](https://doi.org/10.15468/wr3gis)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── checklist-recipe.Rproj : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── data
│   ├── raw                : Source data, input for mapping script
│   └── processed          : Darwin Core output of mapping script GENERATED
│
├── docs                   : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd    : Darwin Core mapping script, core functionality of this repository
    ├── _site.yml          : Settings to build website in docs/
    └── index.Rmd          : Template for website homepage
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `docs/` (advanced)

## Contributors

[List of contributors](https://github.com/trias-project/alien-birds-checklist/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
