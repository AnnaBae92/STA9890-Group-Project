# STA9890-Group-Project
Team 15: Anna Bae, Augustin Nare

The data set is from https://www.kaggle.com/des137/us-births-2018 <br>
I split the data set into 39 csv files and uploaded them due to the size of the original data set. 

The below lines in the our R code will read all the 39 csv files and combine them. 
files = list.files(pattern = "*.csv", full.names = T)
d = do.call(rbind, lapply(files, read.csv))
