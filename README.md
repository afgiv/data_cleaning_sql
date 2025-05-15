#THIS PROJECT IS FOR PRACTICE OR PORTOLIO PURPOSES BUT CAN STILL BE USED FOR ANALYSIS IF NEEDED

This project contains a SQL file and a raw dataset of layoffs of different companies all over the world.

Contents:
'Data_Cleaning.sql' : SQL queries used to clean the data and prepare for analysis and visualization.
'layoffs.csv': The raw dataset containing different companies all over the world that had layoffs from the year 2020 to 2023.

Goals:
To clean the data and prepare for analysis and visualization.
To show confidence, knowledge, and skills on using SQL queries.

Softwares used:
MySQL

Sample queries used:
-- Set the date column to a standard format and change its type to DATE type
                  UPDATE layoffs_staging2
                  SET `date` = STR_TO_DATE(`date`, '%m/%d/%Y');
                  
                  ALTER TABLE layoffs_staging2
                  MODIFY COLUMN `date` DATE;
