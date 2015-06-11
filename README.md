# Loading-CSV-dataset-into-MySQL-Database
There are a skill for MySQL reading CSV-dataset  

#Create a CSV format for loading into MySQL

create table yourdata(

title form NOT NULL,
title1 form NOT NULL,

PRIMARY KEY (`title`,`title1`)
)

CHARACTER SET utf8 COLLATE utf8_unicode_ci; // Be able to read character on MySQL


#loading CSV file 
LOAD DATA INFILE "Directory"
INTO TABLE yourdata
COLUMNS TERMINATED BY ','
OPTIONALLY ENCLOSED BY '"'
ESCAPED BY '"'
LINES TERMINATED BY '\r\n'
IGNORE 1 LINES
(title,title1);



