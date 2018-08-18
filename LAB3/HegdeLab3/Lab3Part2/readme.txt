scrap_and_make_csv.py contains the code to clean the article data that is scraped from the NYT, it also create a data.csv file that is has Categories and Description columns. 
Categories contains the Categories and the description has the clean articles 

I have read the csv file into a pyspark.dataframe format which lets me do various SQL operations including count according to categories. This is useful to get a word count.

Later I havce used a bunch of libraries to create various stages in the pipeline.

Finally I have fit the data into the pipeline that was create to toconizes and count vectorize. 

This forms the our dataset.
Which is partitioned into training and testing dataset in 70:30 ratio.

Employing 3 classification techniques on the data to get accuracies ranging from 57 to 74 percent.  