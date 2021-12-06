install.packages("here")
library("here")
install.packages('skimr')
library('skimr')
install.packages('janitor')
library('janitor')
library('stringr')
library('readr')
library('dbplyr')
library('tidyverse')

files <- list.files(path='/cloud/project/Fitabase Data 4.12.16-5.12.16')
names <- str_split_fixed(files,"_merged",2)[,1]
for (i in names){
  assign(i,read_csv(paste('/cloud/project/Fitabase Data 4.12.16-5.12.16/',i,"_merged.csv",sep="")))
}
