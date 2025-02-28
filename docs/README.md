# Fairness Awareness: Analysis of Equity in Education
Theo Bakker, The Hague University of Applied Sciences
2025-02-28

<a name="top"></a>

<!-- badges: start -->

<!-- badges: begin -->

<!-- [![](https://img.shields.io/github/last-commit/LTA-HHs/lta-hhs-tidymodels-studiesucces.svg)](https://github.com/LTA-HHs/lta-hhs-tidymodels-studiesucces/commits/main) -->

[![](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![License: Attribution-ShareAlike 4.0
International](https://img.shields.io/badge/license-Attribution--ShareAlike%204.0%20International-blue.svg)](https://cran.r-project.org/web/licenses/Attribution-ShareAlike%204.0%20International)

<!-- badges: end -->

<img src="figures/fairness-awareness-hex.png" align="right" height="160"/>

This <a
href="https://community-data-ai.npuls.nl/groups/view/44d20066-53a8-48c2-b4e9-be348e05d273/project-center-for-educational-data-analytics-ceda"
target="_blank">Npuls CEDA</a> <sup>🔗</sup> project makes it possible
to create a fairness analysis to study equity (*kansengelijkheid*)
within progression of students in educational institutions in The
Netherlands (mbo, hbo, and wo).

## Table of contents

- [About](#-about)
- [Why we study fairness, awareness, and
  equity](#why-we-study-fairness-awareness-and-equity)
- [Getting started](#-getting-started)
  - [Prerequisites for stand-alone
    installations](#prerequisites-for-stand-alone-installations)
  - [Prerequisites for Posit Cloud
    installations](#prerequisites-for-posit-cloud-installations)
  - [Installing](#installing)
- [Rendering your fairness reports](#-rendering-your-fairness-reports)
- [Deployment](#-deployment)
- [Learn more on fairness, awareness, and
  equity](#-learn-more-on-fairness-awareness-and-equity)
- [Built with](#-built-with)
- [Contributing](#-contributing) <!-- - [Versioning](#versioning) -->
- [Authors](#-authors)
- [License](#-license)
- [Acknowledgments](#-acknowledgments)
- [Known issues](#-known-issues)
- [Wishes](#-wished)
- [Contact](#-contact)

## 🎓 About

This R project offers Dutch educational institutions a template for
creating a **fairness analysis of students’ progression in educational
institutions in The Netherlands**. The template is based on the
<a href="https://quarto.org/docs/get-started/"
target="_blank">Quarto</a> <sup>🔗</sup> framework and uses the
<a href="https://www.tidyverse.org/" target="_blank">Tidyverse</a>
<sup>🔗</sup> coding standard. The template is developed by the <a
href="https://www.dehaagsehogeschool.nl/onderzoek/lectoraten/learning-technology-analytics"
target="_blank">Learning Technology &amp; Analytics (LTA)</a>
<sup>🔗</sup> research group of The Hague University of Applied Sciences
for the <a
href="https://community-data-ai.npuls.nl/groups/view/44d20066-53a8-48c2-b4e9-be348e05d273/project-center-for-educational-data-analytics-ceda"
target="_blank">Npuls CEDA</a> <sup>🔗</sup> project.

You will have the option to build two reports. The *advanced fairness
report* you will build, will look like this:

<img src="figures/screenshot-advanced-report.png" align="center" height="300" style = "border: 1px solid #999999"/>

<br/> The *basic fairness report* you will build, will look like this:

<img src="figures/screenshot-basic-report.png" align="center" height="300" style = "border: 1px solid #999999"/>

## 💡 Why we study fairness, awareness, and equity

The Fairness Awareness Template is based on the concepts of Fairness,
Awareness, and Equity. These concepts are essential for the development
of a fair educational system. If we don’t study the fairness of our
institutions, we can’t be aware of the consequences of our actions in
policy, education or student counseling. If we are not aware of the
consequences of our actions, we can’t transform unfair educational
systems.

We use machine learning (ML) models to understand if there is bias in
the progression of students in educational institutions. The fairness of
an ML model can be assessed by examining the quality of its predictions
for different groups of students expressed in fairness metrics. If the
differences in predictions are disproportionally large, this is a sign
of bias within the data, unfairness for some groups of students, and
inequity.

To learn more about the concepts of Fairness, Awareness, and Equity,
read the inaugural speech
<a href="https://zenodo.org/records/14204674" target="_blank">No
Fairness without Awareness</a> <sup>🔗</sup> by Theo Bakker.

## 🚀 Getting started

These instructions will get you a copy of the project up and running on
your local machine for development and testing. See the
[deployment](#deployment) for notes on deploying the project on a live
system.

### Prerequisites for stand-alone installations

To start working with this project, make sure you have the following
software installed following the links provided, unless you use a paid
version of Posit Cloud:

**R, Rstudio, Quarto, XQuartz (for Mac only)**

- RStudio version 2024.12.0 or higher with R version 4.4.2 or higher -
  <a href="https://posit.co/download/rstudio-desktop/"
  target="_blank">Posit</a> <sup>🔗</sup>
- XQuartz 2.8.5 or higher (for Mac only) -
  <a href="https://www.xquartz.org/" target="_blank">XQuartz</a>
  <sup>🔗</sup>
- Quarto version 1.6.39 or higher -
  <a href="https://quarto.org/docs/get-started/"
  target="_blank">Quarto</a> <sup>🔗</sup>. Since we use the latest
  Quarto functionalities, you will need at least this version.

**Github, GitHub Desktop**

- A Github account and (optionally) GitHub Desktop version 3.4.16 - <a
  href="https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/installing-github-desktop"
  target="_blank">Github</a> <sup>🔗</sup>

**GFortran**

- GFortran -
  <a href="https://fortran-lang.org/learn/os_setup/install_gfortran/"
  target="_blank">Fortran</a> <sup>🔗</sup>. Fortran is needed to work
  with several machine-learning packages. Installation will take several
  minutes. You might have to restart your computer after installation.

**R packages, fonts**

- Other packages are installed automatically by running the project on
  your local machine. Instructions are below.
- The installation of the Liter font is optional. Follow the
  instructions from Google to install this font. -
  <a href="https://fonts.google.com/specimen/Liter"
  target="_blank">Google</a> <sup>🔗</sup>

### Prerequisites for Posit Cloud installations

- Login into Posit Cloud and create a `New Project from Git Repository`.
- Copy and paste the following url
  https://github.com/LTA-HHs/lta-hhs-fairnessawareness/. That’s it.

### Installing

1.  First, make a fork of the repository to your own Github account. A
    fork is a copy of the original repository you create in your own
    GitHub account. This allows you to modify it independently without
    affecting the original project. Then clone the repository to your
    local machine using for instance GitHub Desktop. See <a
    href="https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository"
    target="_blank">Cloning a repository</a> <sup>🔗</sup> for an
    explanation.
2.  Once you have cloned the repository, open the project in RStudio and
    run the `_Setup.R` file by clicking on `Source`. Don’t change any
    settings yet. This action will install all the necessary packages
    and fonts. This installation process will take about 5-10 minutes.
3.  Ignore any inline suggestions at the top of R Studio to install
    missing packages. Click on `Don't show again`
4.  When presented with the following question, choose 1.

``` plaintext
It looks like you've called renv::restore() in a project that hasn't been activated yet.
How would you like to proceed? 

1: Activate the project and use the project library.
2: Do not activate the project and use the current library paths.
3: Cancel and resolve the situation another way.
```

5.  Your session will restart. Run the `_Setup.R` file by clicking on
    `Source`.
6.  Answer all questions about installations with Yes (Y or y).
7.  Once you have all the packages installed, it is best to restart your
    R session.

## 📚 Rendering your fairness reports

- Follow the [Tutorial](TUTORIAL.md) to learn more about why we study
  fairness, and how to create and render your institutional fairness
  reports.

## 🔨 Built with

- <a href="https://quarto.org/docs/get-started/"
  target="_blank">Quarto</a> <sup>🔗</sup> - The web framework used with
  R.
- <a href="https://www.tidyverse.org/" target="_blank">Tidyverse</a>
  <sup>🔗</sup> - The R coding standard used.
- <a href="https://www.tidymodels.org/" target="_blank">Tidymodels</a>
  <sup>🔗</sup> - The R package used to build the prediction models.
- <a href="https://dalex.drwhy.ai/" target="_blank">Dalex</a>
  <sup>🔗</sup> - The R package used to explain the prediction models
  and create the fairness analysis. The implementation of the fairness
  analysis is based on the
  <a href="https://fairness.drwhy.ai/" target="_blank">Fairness</a>
  <sup>🔗</sup> package.

The LTA-HHs team adjusted the Dalex implementation to improve usability
and make it suitable for use in the educational sector in the
Netherlands.

## 🔧 Contributing

In the next version of this template, we will explain how you can
contribute to this project. Until then, please get in touch with Theo
Bakker if you have any suggestions.

<!-- ## 🔩 Versioning -->

<!-- We use [SemVer](http://semver.org/) for versioning. See the [tags on this repository](https://github.com/LTA-HHs/lta-hhs-fairnessawareness/tags) for the available versions.  -->

## ✒️ Authors

- **Theo Bakker**, Professor of Learning Technology & Analytics of The
  Hague University of Applied Sciences (THUAS), t.c.bakker@hhs.nl -
  *Initial work* -
  <a href="https://github.com/tcbakker" target="_blank">Theo Bakker</a>
  <sup>🔗</sup> and
  <a href="https://github.com/LTA-HHs" target="_blank">LTA-HHs</a>
  <sup>🔗</sup>

## 🚦 License

This project is licensed under the [Creative Commons Attribution Share
Alike 4.0 International](LICENSE.md).

## 🔆 Acknowledgments

- We want to thank the developers of Quarto, Tidyverse, Tidymodels and
  Dalex for their excellent work.
- We want to thank Npuls and CEDA for their support in developing this
  template.

## 📌 Known issues

- None

## 📎 Wishes

- Be able to include logo in \_brand.yml for subsequent use in
  basic.scss.
- Remove Warnings while rendering .qmd files without parameters

## 📫 Contact

If you have any questions or suggestions, please contact the author of
this template: [Theo Bakker](mailto:t.c.bakker@hhs.nl)

*To the [version history of the template](NEWS.md).*

[Back to top](#top)
