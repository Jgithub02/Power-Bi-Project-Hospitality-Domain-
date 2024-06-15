# Power-Bi-Project-Hospitality-Domain-

# Problem Statement: 
AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands is losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of AtliQ Grands wanted to incorporate “Business and Data Intelligence” to regain their market share and revenue. However, they do not have an in-house data analytics team to provide them with these insights.

Their revenue management team had decided to hire a 3rd party service provider to provide them with insights from their historical data.
# Steps Followed 
# Data Loading: 
Load the data into Power BI from MS Excel. 
# Data Transformation: 
Data transformation Using Power Query 
![data transformation ](https://github.com/Jgithub02/Power-Bi-Project-Hospitality-Domain-/assets/164842901/e616d647-851a-4b4b-a48f-4e8d7c9ae3f1)
# Data Analysis Expression :
Using DAX created new columns 
<br> 
In the dim_date data table, I had created two new columns "wn" and "day type" using the following formulas-
<br>
```wn = WEEKNUM(dim_date[date])``` 
<br>
```
day type = 
 
 Var wkd = WEEKDAY(dim_date[date],1)

 return
 IF(
 wkd>5,"Weekend","Weekday")```



