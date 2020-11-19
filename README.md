# Project Three Customer Churn for SyriaTel

[Slides and Presentation Folder](https://drive.google.com/drive/folders/1NddLHopNLhAqZx7mU4sF_FbB-gEAjrpo?usp=sharing)

### Strategic Approach

For this project, I have been tasked with finding the strongest indicators of sale price in the King County Dataset using linear regression techniques that I completed in Module 2 from the Flatiron Data Science Full Time Course.

I've defined my stakeholders as construction developers or real estate developers who are interesting in profiting from building property in the King County area. Information provided online at kingcounty.gov disclose that from 2010 to 2018 the population rose by roughly 400,000 people. Considering that this isn't a high growth rate, this may result in the inability to quickly sell properties which can be a hindrance to developers. Due to this inconvenience, developers would most likely be interested in:

 - Long term investment of building property and renting it out.
 - Long term investment of building commercial strip centers and renting them out.

### The Data

The data used was from the King County House Sales dataset. Additionally I pulled average income by zipcode from https://www.incomebyzipcode.com.


### Question One

[Question One Notebook Link](https://github.com/jaykayso/dsc-phase-2-project-online/blob/master/Notebooks/Module%202%20Question%20One%20Final%20Draft.ipynb)
<summary style="font-size: 24px">
Question 1: What features are contributing most aggressively to the sale price?
    
I got an r-sqared value of .928 in my OLS model by using feature engineering. I engineered features for latitudinal distance to North Mercer Island, and income by zipcode. Narrowing down the features by high pvalue and low coefficient values allowed me to determine the 3 most influential features for predicting the sale price. 
    
The 3 most influential features were: 
- sqft_living: The indoor square footage.
- lat_dist: The latitudinal distance from N. Mercer Island. 
- income: Average income by zipcode.
    
### Conclusion

In conclusion, large property sizes are indicative of higher sale prices, so given a lot to build on, our stakeholders may to make a larger indoor area and smaller lot. Since income is a factor in sale price, budgets for building projects should be configured so that asking prices are relative to income prices in the area. Additionally further analysis could be implemented to standardise the features and determine how the features compare to each other when determining sale price. 

### Question Two

[Question Two Notebook Link](https://github.com/jaykayso/dsc-phase-2-project-online/blob/master/Notebooks/Module%202%20Question%20Two%20Final%20Draft.ipynb)
<summary style="font-size: 24px">
Question 2: What property types are most common?

To further understand the properties that have prices affected by the aforementioned features, I looked into the most common sale prices, most common property types, and the area where the most properties sold. 
    
The most common sale price is around $350,000. The data forms a normal distribution that skews right. 
    
The most common number of bedrooms is 3 or 4.
Out of the 3 bedroom properties, the most common number of bathrooms is 1, 1.75, and 2.5.
Out of the 4 bedroom properties, the most common number of bathrooms is 2.5.
    
The area with the most sales was the zip code of 98199.

### Conclusion

In conclusion, understanding the types of properties that are most common can help in determining the demand in the market. However, this does not determine true demand in the market and futher analysis could be used to determine competition, properties currently for sale, properties that sell the most quickly, or other factors that indicate the supply and demand of the market. This information could then be leveraged to determine properties that could be sold quickly, which would be preferred for a developer.  

### Question Three
    
[Question Three Notebook Link](https://github.com/jaykayso/dsc-phase-2-project-online/blob/master/Notebooks/Module%202%20Question%20Three%20Final%20Draft.ipynb)
<summary style="font-size: 24px">
Question 3: What percentage of properties have all of the aforementioned attributes?

By splicing the data, I determined that all of the properties in the zipcode of 98199 with 3 or 4 bedrooms sold for over $350,000(the most common price). None of the properties had all of the most common attributes.
    
### Conclusion
    
In conclusion, these findings determine that the demand is not obvious. It shows that the property types are not homogenous and vary greatly. Further research based on the unique goals of the developers could be used to analyse the profit potential in the market. 

    
# Conclusion and Future Work
    
Our developers should consider building properties with small outdoor areas to maximize the indoor square footage. Additionally the asking price should be relative to the average zipcode in the area. Since there is variation in the properties, further analysis would be useful in analyzing the market to better understand supply and demang. Those findings could be used in association with the goals of the developers to find opportunities with the best profit potential. 
 
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    