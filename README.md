Predicting Hazardous NEOs (Near-Earth Objects)
📌 Project Overview
This project focuses on predicting whether a Near-Earth Object (NEO) is hazardous or not using a dataset provided by NASA. The goal is to build a machine learning model that can accurately classify NEOs as hazardous or non-hazardous, which is crucial for planetary defense and space monitoring.

Dataset Description
The dataset includes the following key features:

Absolute Magnitude: The brightness of the NEO.
Estimated Diameter: The minimum and maximum estimated diameter of the NEO.
Relative Velocity: The velocity of the NEO relative to Earth.
Miss Distance: The distance by which the NEO missed Earth.
Orbiting Body: The celestial body that the NEO is orbiting.
Is Hazardous: The target variable indicating whether the NEO is hazardous (1) or not (0).
Project Steps
1. Data Importing and Cleaning
The dataset was loaded and missing values were handled by filling them with the mean of the respective columns.
Duplicate rows were removed to ensure data quality.
2. Exploratory Data Analysis (EDA)
The distribution of the target variable (is_hazardous) was analyzed to understand the balance between hazardous and non-hazardous NEOs.
A correlation heatmap was created to explore relationships between numerical features such as diameter, velocity, and miss distance.
3. Data Preprocessing
Categorical variables, such as the orbiting_body, were encoded to prepare the data for machine learning models.
The dataset was split into training and testing sets to evaluate model performance.
To address the imbalance in the target variable, SMOTE (Synthetic Minority Over-sampling Technique) was applied to balance the classes.
4. Model Training and Evaluation
A Random Forest Classifier was trained on the preprocessed data due to its ability to handle complex relationships and high accuracy.
The model was evaluated using key metrics such as Precision, Recall, F1-Score, and AUC-ROC Score.
The ROC curve was plotted to visualize the model's performance in distinguishing between hazardous and non-hazardous NEOs.
Results & Insights
The model achieved an AUC-ROC score of 0.99, indicating excellent performance in classifying hazardous NEOs.
The confusion matrix showed high accuracy, with very few false positives and false negatives.
Key insights from the model include:
The most important features for predicting hazardous NEOs are relative velocity, miss distance, and absolute magnitude.
The model can effectively identify hazardous objects, which is critical for planetary defense strategies.
Repository Structure
bash
Copy
Edit
📂 predicting_hazardous_neo_project
│-- 📂 data/               # Contains raw and processed data files
│-- 📂 notebooks/          # Jupyter Notebooks for data analysis and modeling
│-- 📂 reports/            # Visualized reports and insights
│-- README.md             # Project documentation
│-- requirements.txt      # List of dependencies and libraries used
How to Run the Project
Install the required dependencies:
sh
Copy
Edit
pip install -r requirements.txt
Open the Jupyter Notebook to preprocess the data, train the model, and evaluate its performance.
Explore the visualizations and insights generated during the analysis.
Technologies Used
Python for data analysis and machine learning.
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, and Imbalanced-learn.
Machine Learning Algorithms: Random Forest, SMOTE for handling imbalanced data.
Conclusion
This project successfully developed a highly accurate machine learning model to predict hazardous NEOs. By leveraging advanced data preprocessing and machine learning techniques, the model can effectively identify potentially dangerous objects near Earth. This tool can be invaluable for space agencies and researchers focused on planetary defense and space monitoring.

👨‍💻 Author
Sondos Sofian
📧 Contact: sondosso889@gmail.com
