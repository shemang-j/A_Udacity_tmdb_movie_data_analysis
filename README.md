# tmdb-movies data analysis

In this project we will be analysing the dataset tmdb-movies.csv, This data set contains information about 10,000 movies collected from The Movie Database (TMDb), including user ratings and revenue.

## Question of analysis

In this project we would be finding insights about which year generated the highest average revenue in movie production From the year 2000 to the year 2015 for both comedy and drama? only Also, we would find the genre with the highest budget in the year 2010 between the genres comedy and drama.

## Packages used 

* pandas
* Numpy
* matplotlib
* seaborn

## data wrangling

The code below was used to obtain movies produced from the year 2000 to 2015
```
mask_1 = df["release_year"] >= 2000 #Obtaining the release_year of 2000 and above 
df = df[mask_1]                     #using the indexing and selecting data method
df.head()
```
Null values and unwanted columns were dropped

## data exploration

Functions plot_bar_by(x, xlabel, ylabel, title) and plot_stacked_bar(x, xlabel, ylabel, title) were created to plot visuals

## Conclusions

In the data visualization exploration that we have created we could see that for our first research question it shows that the year 2000 had the highest revenue of about 60000000 and the drama movies in that year 2000 had the highest average revenue of about 70000000 compared to drama, aslo the revenue decreases over the years   
Secondly, for the second research question in the year 2010 between the genres comedy and drama, comedy had the heighest budget of about 1500000. Also the year 2003 had the highest budget of about 20000000 and the budget decrease over the years
Lastly, their were limitation in our analysis because, The important variables in the dataset which are budget and revenue includes 0.0 values until the 50% percentile this means half of the data in these columns are 0.0. this might be as a result of missing data and 0.0 was used to input it.
therefore can not be used to generalised the whole data set

