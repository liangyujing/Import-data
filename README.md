# Clear workspace
rm(list=ls())

# Set your working dir as the current dir
setwd(dirname(rstudioapi::getSourceEditorContext()$path))

# read data csv file
library("readr")

my_data <- read_csv(file.choose())   ##自己选文件

my_data <- read.csv(file="R code/antisemitism_07.csv", head=T,sep=";")   ##列不会合并，有sep
my_data <- read_tsv("mtcars.txt", sep="")
my_data <- read.table("bloodtype.txt", header=TRUE, sep="")  
my_data <- read.delim(),   #TXT

summary(my_data)

# EXCAL   Use readxl package to read xls|xlsx
library("readxl")
my_data <- read_excel("my_file.xlsx")

dim(my.data)
names(my.data)

