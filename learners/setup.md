---
title: Pre-workshop Setup
---

<h2><b>PART I:Install Git and create GitHub Account</b></h2>

We will need the following account(s) and software for this workshop:

- Create Github account (use existing or create new account)
- Install Git
- Install R \& RStudio (Two separate installations: if you are on a windows device, you may need <a href="https://cran.r-project.org/bin/windows/Rtools/">Rtools</a>)

{% include install\_instructions/github.html %}

{% include install\_instructions/git.html %}

<br>

<h2><b>PART II: Install R/Rstudio and Quarto</b></h2>

{% include install\_instructions/r.html %}



<br>

## Quarto

Quarto is a scientific and technical publishing system build on Pandoc, which we will be using in Rstudio.
You will need to install Quarto from <a href="https://quarto.org/docs/get-started/">Quarto.org</a>. Open the Setup Wizard to begin the install.
Keep the defaults and select <b>Next</b> until the install finishes.

:::::::::::::::::::::::::::::::::::::::  keypoints

## Version clarifications on Quarto and R/Rstudio

::::::::::::::::::::::::::::::::::::::::::::::::::

If you already have Rstudio and R installed, please check if you have the most updated <b>2023\.06</b> Rstudio and at least R version <b>4\.3</b>, along with Quarto version <b>1\.3.45</b>. The quarto document will not render without the most updated versions. <b>The Quarto Package is not the CLI</b>


<br>

You can check if you have the correct Quarto version by typing the following in the Rstudio terminal:

```source
quarto --version
```

Your output should be:

```output
quarto --version
1.4
```

<br>

## R Packages

Install the following packages in RStudio: `rmarkdown`, `tidyverse`,`BayesFactor`, `patchwork`.
We will be covering the purpose of using packages and recap different ways to install and manage them in RStudio. Nonetheless, pre-installating the packages we will be using for this workshop will save us some precious time since installation time may vary among learners. Here are the steps for two possible approaches you may follow for completing this process:

*Using Menus and Tabs*

1) Open R studio

2) Select from the upper menu `Tools > Install packages...` or click on the `Packages` tab in the bottom-right section and then click on install. Either action will prompt a box dialog.

3) In the `Install Packages` dialog box, copy this command `rmarkdown, tidyverse, BayesFactor, patchwork` under the Packages field, make sure the option `install dependencies` is selected, keep other information unchanged, and then click `install`.

4) Don't be alarmed by the stop sign that will blink (and do not click on it otherwise you will cancel the process) or the red text messages. Once the process completes the cursor will be preceeded by a greater-than sign `>`.

5) Copy and paste one of the following functions to the console and wait for the process to complete:

```source

 install.packages("rmarkdown")
 install.packages("tidyverse") 
 install.packages("BayesFactor") 
 install.packages("patchwork")

```

or

```
  
 install.packages(c("rmarkdown", "tidyverse", "BayesFactor", "patchwork"))
```


