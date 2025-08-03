# Nutriplan-Personalized-Nutrition-and-Diet-Planning-Using-AI
NutriPlan is a web-based application that uses Al and the Nutritionix database to offer personalized dietary recommendations. Users input their goals and preferences, and the system provides food suggestions and nutritional analysis. Key features include food logging, real-time calorie and nutrient tracking, and Al-driven recommendations tailored to individual needs, simplifying the process of managing nutrition.
## Project Architecture
<img width="700" height="700" alt="image" src="https://github.com/user-attachments/assets/bd2b13e4-7929-4437-bb57-a697dca0470d" />

Installation Guide

1.Install python 3.

2.Install flask using 
```bash
pip install flask
```

3.Navigate to your project directory

4.Run the server using 
```bash
python flask_server.py
```

Usage

Adding a Food

This page enables users to add food items to their food log. Using the Nutritionix NLP API, the query can include multiple food items at once, which will be added to the results table. When the double arrow icon is clicked, the nutrition facts are displayed on the nutrition label. Users can then select the time and date to log the food. Additionally, when searching for foods, the system adds them to our local database. A feature extraction algorithm is applied to categorize the foods as high or low in macronutrients. This information will later be utilized for generating food suggestions.

![Screenshot 2025-03-17 144511](https://github.com/user-attachments/assets/1f664d65-5791-4c34-bdcd-5102a322c5d3)

Food History Log

This page displays the user's food history for the selected day. Once the data is loaded, users can delete items from their history by clicking the delete icon. Feedback is integrated through labels in the history tab. By clicking on the labels, the decision tree algorithm is revealed, showing users how the label was determined, incorporating explainable AI.

![Screenshot 2025-03-17 144601](https://github.com/user-attachments/assets/b774f53a-99c0-4f35-826c-3f145646c9c6)

Tracking Nutrition

This page displays the macronutrient breakdown for the selected day. Users can choose a specific day and select a graph type (bar, pie, or line) to visualize their macronutrient distribution for that day. The food suggestions will also be loaded, allowing users to see how adding certain foods will impact their nutrient breakdown. If a user clicks the trash icon, the item will be added to a "do not suggest" list, ensuring that these foods are not suggested in the future.

![Screenshot 2025-03-17 144647](https://github.com/user-attachments/assets/600840ee-f22f-4f43-a772-fb0bba861a7c)

User Preferences

This page enables users to create their own personalized diet plan and set preferences. Recommended macronutrient values are provided, and users can adjust these values as needed using sliders to tailor their diet plan.

![Screenshot 2025-03-17 144712](https://github.com/user-attachments/assets/a5d0a0ee-6d5d-4bdb-99d2-31d1efadd345)

Recipe suggestions

Recipe suggestions are provided based on dietary preferences, including options for vegan, vegetarian, and non-vegetarian meals.

![Screenshot 2025-03-17 144740](https://github.com/user-attachments/assets/a3cf1d39-4059-497f-8db1-64373e165caa)




