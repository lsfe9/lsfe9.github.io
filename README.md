# lsfe9.github.io

# Intro of my repository
This repository contains my quarto website for DSCI 521. There are 2 new analysis post about the Palmer Penguins dataset which written in different coding languages Python and R.

# Installation requirements
1. quarto --version 1.10.18
2. uv --version 0.12.7
3. R --version 4.6.1
The required Python packages are recorded in `uv.lock`, and the required R packages are recorded in `renv.lock`. Also, renv bootstraps itself.

# Build the website
You could run the following commands in your Git Bash terminal to built site.

cd yourfolder
git clone https://github.com/lsfe9/lsfe9.github.io.git
cd lsfe9.github.io
uv sync
R 
renv::restore()
q()
n
uv run quarto render

# Open the site locally
The rendered website is in the `docs` folder. Open `docs/index.html` in a web browser, then you can see the website. These posts are under `docs/posts`.

# Data Source
For both Python and R analysis, I used the Penguins data from the `palmerpenguins` package. If you have install all the required package in the Installation requirements steps,
building the site does not need a network connection to fetch the data.