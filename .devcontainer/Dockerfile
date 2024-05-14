FROM rocker/r-ver:4

# Install system dependencies
RUN apt-get update && apt-get install -y \
    libcurl4-openssl-dev \
    libssl-dev \
    libxml2-dev \
    zlib1g-dev \
    libgit2-dev \
    libfontconfig1-dev \
    libharfbuzz-dev \
    libfribidi-dev \
    libfreetype6-dev \
    libpng-dev \
    libtiff5-dev \
    libjpeg-dev

# Install R packages
RUN R -e "install.packages(c('remotes', 'devtools', 'renv', 'tidyverse', 'languageserver'))"

RUN apt-get update && apt-get install -y \
    git
