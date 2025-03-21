# Milestone 1 (21st March, 5pm)

**10% of the final grade**

This is a preliminary milestone to let you set up goals for your final project and assess the feasibility of your ideas.
Please, fill the following sections about your project.

*(max. 2000 characters per section)*


## Dataset

We have chosen to work with CulinaryDB, which is a structured dataset containing recipes and ingredients for over 22 world regions.

Luckily, the data is of good quality and doesn't need any data-cleaning. However, one issue we might face during our project is the variation in ingredient names due to synonyms. To avoid this, we plan on using the unique ID associated with each  ingredient. 

Only minimal preprocessing is needed, such as removing unnecessary columns and merging the required ones to identify ingredient IDs and names.
CulinaryDB dataset : [Link](https://cosylab.iiitd.edu.in/culinarydb/#databasedescription)


## Problematic

Food is a central part of our world, and understanding the ingredients that define each culture is important to improve our culinary knowledge. Our project aims to visualize the most commonly used ingredients per country and help users find recipes based on their available ingredients in the fridge. 

Tasting Viz will be designed to create an intuitive, visually engaging platform for novice cooks to explore recipes based on the ingredients they have in their fridge, discover new dishes, and develop basic cooking skills.

But before cooking, research is key.  Our website will provide visual insights into our database, highlighting various cooking cultures, the most commonly used ingredients across different cuisines, and much more. Once users gain a solid understanding, they can begin their learning journey by choosing recipes. 

Through this work, our website will answer the users’ following questions: What are the most used ingredients around the world ? How do ingredients relate to one another ? What recipes can be made with specific ingredients? What recipe is the most similar to the one I liked? … and many more. 

As mentioned before, the motivation behind this project is to bridge the gap between ingredient knowledge and culinary skills, making cooking more accessible, exciting, and educational. The target audience includes beginners eager to learn efficient cooking, food enthusiasts looking for inspiration, and anyone aiming to reduce food waste by using ingredients they already have.


## Exploratory Data Analysis

We focused on preprocessing the data by removing ingredients used fewer than once and excluding recipes with fewer than three ingredients. We also explored basic statistics and visualized key trends within the dataset. For a detailed view of our code, graphs, and further analysis, please refer to the "eda" notebook in our repository.

[Noteboook Link](https://github.com/com-480-data-visualization/com-480-project-TastingViz/blob/master/Milestone1/eda.ipynb)

## Related work

### What others have already done with the data?

Most of the previous work on this dataset was done by its original creators. For example, they calculated food pairing scores to compare how well different cuisines pair with each other. Additionally, they performed basic statistics, such as showing the recipe size distribution across different regions, which is a standard practice when starting data analysis.

### Why is your approach original?

To make recipe selection easier and our approach more unique, we will incorporate a search feature that uses our recipe, ingredient, and compound ingredient data. Users can input the ingredients in their fridge or pantry to receive recipe suggestions. Additionally, if you're a picky eater and enjoy a certain recipe, you can search for its closest ingredient neighbors (like cluster) to discover similar ones. 

### What source of inspiration do you take?

Our inspiration comes from a variety of sources, both related and unrelated to cooking.

For our ingredient search tool, we aim to create something similar to the functionality below, but with a more visually appealing design: [source link](https://www.reciperadar.com/)

<p align="center">
  <img src="images/search.png" alt="Search bar" width="700">
</p>

<p align="center">
  <img src="images/search2.png" alt="Search bar" width="700">
</p>


We propose a feature that helps users find similar recipes based on their preferences. When users click on a specific point in the cluster (shown below), a recipe card with the recipe and ingredients will appear, similar to the one on the left.

<p align="center">
  <img src="images/clusters.png" alt="Search bar" width="700">
</p>

Other idea to search through the recipes by recipes or ingredients :  [source 1 link](https://www.pinterest.com/pin/recipe-app-design--791296597023662453/) [source 2 link](https://www.seroundtable.com/google-new-recipe-search-interface-36038.html)

<p align="center">
  <img src="images/search3.jpg" alt="Search example" width="600">
</p>

<p align="center">
  <img src="images/search4.jpg" alt="Search 2 example" width="600">
</p>

Overall, we want our website design to be simple, welcoming, and engaging, similar to the design below: [source link](https://dribbble.com/shots/14787532-Weather-Forecast-Dashboard)


<p align="center">
  <img src="images/theme.png" alt="Search bar" width=700">
</p>


