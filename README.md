# nosql-challenge

This code imports json restaurant data for the United Kingdom then analyzes that data.

## Methods

- Import json data in terminal
- Use pymongo to pull and query the imported database
- Update the database with a new restaurant
- Use find to locate restaurants that fit various parameters

## Database Setup

The data was imported into a mongo database using the following code:
![image](https://user-images.githubusercontent.com/118322354/225806549-4bb34bd3-3bcf-4ad6-bdba-75960f11e9c1.png)

Once the uk_foods database and establishments collection were parsed with mongo and assigned to variables a new restaurant was added to the database with the following code:
![image](https://user-images.githubusercontent.com/118322354/225806782-6f780636-f7f8-46d8-a278-3c07f99a3d82.png)

New information for the new restaurant was deteremined, data types were changed to the appropriate types, and restaurants in locations not of interest were removed.

## Database Analysis

Restaurants with a hygiene score of 20 were queried and the first 10 rows and 8 columns are as follows:
![image](https://user-images.githubusercontent.com/118322354/225807735-b5b4cea1-fdb6-4b93-86c2-54e6eed60f4f.png)

Restaurants in London with a rating of 4 or greater were queried and the first 10 rows and 8 columns are as follows:
![image](https://user-images.githubusercontent.com/118322354/225807932-b9d9c4d0-f6fb-4b2d-a0c8-27e7195d635c.png)

the top 5 establishments with a rating of 5, and within 0.01 degrees of the new restaurant were queried and sorted by lowest hygiene score. The first 8 columns of the results of that query are as follows:
![image](https://user-images.githubusercontent.com/118322354/225808723-56323010-92ac-42c7-9d90-961eea5fe8c9.png)

Restaurants were grouped by local authority and then establishements in those areas with a hygiene score of 0 were counted. The results of that query are as follows:
![image](https://user-images.githubusercontent.com/118322354/225808890-da76b0f4-ed8b-4ade-ab19-123a5d34d297.png)
