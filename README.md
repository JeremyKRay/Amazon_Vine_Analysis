# Amazon_Vine_Analysis
## Overview of the Analysis

The purpose of this project is to analyze the written reviews of the paid Amazon Vine Program. This program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members who are required to publish reviews. This particular project focused on a dataset containing reviews of video game products. PySpark was used to perform the ETL process, including peforming a connection to an Amazon Web Service RDS database to load the data into pgAdmin. Then PySpark was used to determine if there was any bias toward favorable reviews from Vine and non Vine members in the videogame dataset. The results are shown below.

## Results
Below are the results and the code that produced them. 

### How many Vine reviews and non-Vine reviews were there?
  * There were 94 total reviews from Vine members

[![Total Vine.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/Total%20Vine.png)

  * There were 40,471 total reviews from non Vine members

![Total No Vine.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/Total%20No%20Vine.png)

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  * Of the 94 Vine member reviews, there were 48 - 5 star reviews

![Vine 5 star.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/Vine%205%20star.png)

  * Of the 40,471 non Vine member reviews, there were 15,663 - 5 star reviews

![No Vine 5 star.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/No%20Vine%205%20star.png)
   
### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  * 51.06% of Vine members wrote 5 star reviews

![perc 5 star vine.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/perc%205%20star%20vine.png)

  * 38.70% of non Vine members wrote 5 star reviews

![perc_5 star no vine.png](https://github.com/JeremyKRay/Amazon_Vine_Analysis/blob/88f048384839d7860ceb15bdbc9972769d97b6b2/perc%205%20star%20no%20vine.png)

## Summary
The analysis shows that there is a positivity bias in Amazon's Vine Program of 12.36%. Another analysis that could be done would involve looking at other datasets. Since they are all formatted the same, it would not be difficult to join multiple datasets together and perform the same analysis. This would show if this bias is limited to just the video game dataset or if it is consistent across all products. Because there are only 94 Vine members in the video game dataset compared to 40,471 non members, it would be beneficial to include datasets with more Vine members. 
