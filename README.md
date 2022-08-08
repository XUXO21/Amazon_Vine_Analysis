# Amazon_Vine_Analysis
Amazon_Vine_Analysis

---

## 1. Overview of the analysis of the Vine program:

The objective of the project is to analyze Amazon reviews written by members of the paid Amazon Vine program, which allows manufacturers and publishers to receive reviews for their products. In this project, we gor acces to cameras dataset and by the use of PySpark we performed the ETL process to extract the dataset, transform the data, connect to AWS RDS instance, and then load the transformed data into pgAdmin. Next with the use of PySpark we determined if there is any bias toward favorable reviews from Vine members.

## 2. Results:

### ETL Process:

* Customer Table

![C](/Resources/1customertable.png)

* Products Table

![P](/Resources/2productstable.png)

* Review ID Table

![R](/Resources/3reviewidtable.png)

* Vine Table

![V](/Resources/4vinetable.png)

* SQL PGAdmin example Tables:

![C2](/Resources/customertablepgadmin.png)

![V2](/Resources/4vinetablepgadmin.png)

### 1,801,974 Total Reviews

![TR](/Resources/Totalreviews.png)

* Vine reviews: 607 / non-Vine reviews: 50,522

![PandNP](/Resources/paidunpaiddescribe.png)

* Vine 

** 5 stars reviews: 257
** Percentage of Vine reviews 5 stars: 42.3%

![V](/Resources/Paiddata.png)

* Non-Vine

** 5 stars reviews: 25,220
** Percentage of Non-Vine reviews 5 stars: 49.9%

![TR](/Resources/Unpaiddata.png)

## 3.Summary: 

To start the number of Vine reviews is only 607 from 1,807,974 reviews. It is very small and not represntative. Now taking this information as directional we can say:

- We can't see bias since the average star ratinf is very similiar on both Vine and Non-Vine Users (Vineaverage rating: 4,09 & Non-Vine average rating: 3.86), also 5 star reviews percentage is higer on Non-Vine users is higer than on Vine ones (Vinea rating: 42.3% Non-Vine rating: 49.9%)

We should create an additional Analysis not only using more cagtegories to compare, maybe the camara category is an outlayer on the total products information. Maybe undestanding the sentiment of the reviews could help to the if it is more positive on Vine suscriptors vs the Non-Vine.
  
