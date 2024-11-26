# Template for writing a handout or a presentation

This repository contains a Quarto template. This template was created for my course "Data Analysis for Decision-Making", which I held for the University of Applied Science Fresenius. 

# Download the repo

## Method 1: Using the mouse

### Method 1a: Clicking in GitHub

In GitHub, click on the green `<> Code v` button found in this repository. In the context menu that opens, you will find a button called `Download ZIP`. Click on it and you will have a zipped copy of the repo that you can unzip and use.

### Method 1b: Click on [this link](https://github.com/hubchev/dadm_guide2425/zipball/HEAD)

You can download the repository in a zipped file using [this link](https://github.com/hubchev/dadm_guide2425/zipball/HEAD). Now you can unzip it to a directory of your choice.

## Method 2: Using R

### Method 2 a): `quarto_use_template()`

If you have installed the R package `quarto`, the template can be copied with the function `quarto_use_template`. To do this, set your working directory to the directory in which you want to install the template (e.g. `setwd("path/to/my/folder")`). Make sure that the directory is empty and execute this command:

```{r}
quarto::quarto_use_template("hubchev/dadm_guide2425")
```

A prompt will ask if you trust the author (me) not to execute malicious code. To continue, reply with `Yes` or simply `Y`.

### Method 2 b): usethis::use_course()

Install and download the usethis package and download it with `use_course`:

```{r}
install.packages("usethis")
library("usethis")
usethis::use_course("hubchev/dadm_guide2425", destdir = getwd())
```

By default, the repository is downloaded to a directory and stored in your working directory. Feel free to replace `getwd()` with "path/to/target", i.e. the desired location on your system where you want to download the repository.


## Method 3: Using the terminal
### Method 3a: Using Git

If you have Git installed on your system ([here](https://git-scm.com/downloads) you can download it if necessary), you can download this repository using the command line:

- Open the terminal in R Studio (In RStudio, the terminal is in a tab next to the console.) or the command prompt window of your operating system.
- Navigate to the directory where you want to download the repository using the cd command (e.g. `cd ~/documents`).
- Execute the following command to clone the repository:

```{bash}
git clone https://github.com/hubchev/dadm_guide2425.git
```

### Method 3a: Using Quarto

Use the terminal (In RStudio, the terminal is located in a tab next to the console.) to navigate to the directory where you want to copy the template (e.g. cd path/to/my/folder). Make sure the directory is empty and execute this command:

```{bash}
quarto use template hubchev/dadm_guide2425
```


# Using the template

Once you have downloaded the repository, navigate to the directory where you downloaded it and open the `temp_apa_en.qmd` file in RStudio or your favorite editor. Customize the template to create your own work!

To convert the Quarto file into the desired document (e.g. a PDF or HTML), "render" the `.qmd` file of your choise. You can do this in RStudio by opening the file and clicking on the "Render" button or by executing the following command in the R console:

```{r}
quarto_render("path/to/dadm_handout.qmd")
```

Replace "path/to/temp_apa_en.qmd" with the actual path to the file.


# Feedback

If you have any questions or need help with the template, feel free to `pull request` changes via GitHub or contact me. 