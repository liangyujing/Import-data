# Clear workspace
rm(list=ls())

# Set your working dir as the current dir
setwd(dirname(rstudioapi::getSourceEditorContext()$path))

# read data csv file
library("readr")
my_data <- read_csv("mtcars.csv",sep = ";")
my_data <- read_tsv("mtcars.txt")
my_data <- read.delim(),   #TXT
my_data <- read.table()
# EXCAL   Use readxl package to read xls|xlsx
library("readxl")
my_data <- read_excel("my_file.xlsx")

dim(my.data)
names(my.data)
