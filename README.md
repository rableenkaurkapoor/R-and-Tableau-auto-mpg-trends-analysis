# R-Tableau-auto-mpg-trends-analysis

This project analyzes how automobile engine characteristics influence fuel efficiency (MPG) using statistical analysis in R and data visualization in Tableau. The workflow begins with statistical exploration and regression analysis in R, followed by visual exploration and dashboard creation in Tableau to communicate insights effectively.

---

# 1️⃣ Statistical Analysis using R

The first stage of this project involved performing statistical analysis in R to understand how engine-related factors impact vehicle fuel efficiency (MPG).

Using the Auto MPG dataset, several engine characteristics were examined, including:

- Horsepower
- Weight
- Displacement
- Cylinders
- Model Year
- Origin

---

## Data Preparation

Before conducting statistical analysis, the dataset required preprocessing:

- The horsepower column contained missing values represented as "?"
- Horsepower values were converted to numeric format
- Missing horsepower values were replaced using the median to reduce the effect of outliers

---

## Statistical Analysis in R

Using R, the following analytical steps were performed:

- Exploratory data analysis of the Auto MPG dataset
- Summary statistics of engine variables
- Linear regression analysis to examine how engine factors influence MPG
- Evaluation of relationships between MPG and variables such as horsepower, weight, displacement, cylinders, and model year

These statistical results provided an analytical understanding of which engine characteristics most strongly influence fuel efficiency.

---

# 📊 Exploratory Data Analysis Visualizations (R)

## Scatter Plot: MPG vs Horsepower

<img width="859" height="593" alt="image" src="https://github.com/user-attachments/assets/557d19b0-ef88-4513-b612-7fca043f7ab0" />

**Explanation**

· This scatter plot shows the relationship between a car’s horsepower (x-axis) and its fuel efficiency, measured in miles per gallon or MPG (y-axis).  
· Each dot represents a car from our dataset of 398 vehicles.  
· The key pattern here is a clear negative correlation: as horsepower increases, MPG generally decreases. In other words, cars with more powerful engines tend to be less fuel-efficient.  
· For example, cars with lower horsepower-under 100-often achieve over 30 MPG. In contrast, cars above 150 horsepower rarely exceed 20 MPG.  
· This trend is expected: higher horsepower means the engine uses more fuel to deliver greater performance, which reduces efficiency.  
· This insight was confirmed through our simple linear regression analysis, where we found that horsepower alone explains a significant portion of the variability in MPG.  
· Overall, this plot visually supports our finding that horsepower is a strong negative predictor of fuel efficiency.

---

## Scatter Plot: MPG vs Weight

<img width="859" height="583" alt="image" src="https://github.com/user-attachments/assets/161e1b28-ff8e-46e4-8986-a5d3616d33fe" />

**Explanation**

· This scatter plot shows the relationship between a car’s weight (x-axis) and its fuel efficiency, measured in miles per gallon or MPG (y-axis).  
· Each point represents a car from our dataset. The overall pattern reveals a strong negative correlation: as weight increases, MPG decreases.  
· Heavier cars, especially those above 4000 pounds, typically achieve lower MPG-often below 20. In contrast, lighter cars under 2500 pounds frequently exceed 30 or even 40 MPG.  
· This makes intuitive sense: heavier vehicles require more energy to move, so they consume more fuel and are less efficient.  
· Among all features we explored, weight is one of the strongest predictors of fuel efficiency. This was confirmed in our regression analysis, where weight had a significant negative impact on MPG.  
· In summary, the plot highlights that reducing vehicle weight is a key strategy for improving fuel efficiency.

---

## Box Plot: MPG vs Number of Cylinders

<img width="861" height="579" alt="image" src="https://github.com/user-attachments/assets/0e0e3658-251d-42ce-85f0-9a47ed6b33c0" />

**Explanation**

· This boxplot shows how fuel efficiency, measured in miles per gallon (MPG), varies with the number of engine cylinders in each car.

Main Trend:

· Cars with fewer cylinders-especially 4-cylinder engines-have much higher MPG.  
· The median MPG for 4-cylinder cars is the highest, and there are several very fuel-efficient outliers in this group.  
· As the number of cylinders increases to 6 or 8, the median MPG drops significantly.  
· 8-cylinder cars have the lowest MPG and the least variability.  

Key takeaway:

· Fewer cylinders generally mean better fuel efficiency.  
· This supports the idea that smaller, simpler engines use less fuel.

---

# 📉 Regression Model Diagnostics

## Residual Plot

<img width="1013" height="685" alt="image" src="https://github.com/user-attachments/assets/b2a14563-d150-48f8-86c4-6b73677fb407" />

**Explanation**

· This plot shows the difference between the actual and predicted MPG values for each car in the test set.  
· Residuals represent the errors between actual and predicted MPG values.  
· Ideally, residuals should be randomly scattered around the zero line.  
· Most points are clustered around zero, indicating that the model’s predictions are generally unbiased.  
· There are some larger residuals where the model underestimates MPG for a few vehicles.  

Summary:

· The residual plot confirms that the regression model provides a reasonable fit for predicting MPG.

---

## Histogram of Residuals

<img width="1013" height="688" alt="image" src="https://github.com/user-attachments/assets/317e3ae2-223e-4520-9296-a6d75f4c130d" />

**Explanation**

· This histogram shows the distribution of residuals from the regression model.  
· Residuals are the differences between the actual and predicted MPG values.

Interpretation:

· Most residuals are clustered close to zero, meaning the model’s predictions are generally accurate.  
· The distribution is roughly bell-shaped but slightly skewed to the right.  
· This suggests the model slightly underestimates MPG for some vehicles.

Summary:

· Overall, the model performs well for most observations, though there are a few outliers.

---

# 📊 Key Statistical Insights

Across all three analyses, several consistent patterns emerge:

- MPG decreases as horsepower increases
- Heavier vehicles tend to have lower MPG
- Cars with fewer cylinders achieve higher fuel efficiency
- Engine size and vehicle weight are key factors affecting fuel consumption

These insights guided the next stage of the project, where Tableau was used to visualize the patterns and create an interactive dashboard.

## 2️⃣ Data Visualization using Tableau

After completing statistical analysis in R, the dataset was visualized using Tableau to better understand and communicate the relationships between engine characteristics and MPG.

Interactive scatter plots were created to visually explore how different variables influence fuel efficiency.

### Visualizations Created

https://public.tableau.com/app/profile/rableen.kaur/viz/DASHBOARD-AnalyzingAutomobileEngineImpactonMPG/DASHBOARD-AnalyzingAutomobileEngineImpactonMPG?publish=yes

<img width="784" height="630" alt="image" src="https://github.com/user-attachments/assets/58070359-c54e-4fd8-84ae-73647c10b342" />


The following visualizations were developed in Tableau:

- Scatter Plot: MPG vs Horsepower  
- Scatter Plot: MPG vs Weight  
- Scatter Plot: MPG vs Displacement  
- Scatter Plot: MPG vs Model Year  

These visualizations help clearly reveal patterns between engine features and fuel efficiency.

---

## 📊 Tableau Visualizations

### MPG vs Horsepower

<img width="508" height="619" alt="image" src="https://github.com/user-attachments/assets/48566293-202a-4880-83cf-bad0885db500" />

### MPG vs Weight

<img width="512" height="612" alt="image" src="https://github.com/user-attachments/assets/b09736e6-c3f4-4630-b6e4-d9cda2d31afc" />

### MPG vs Displacement

<img width="512" height="608" alt="image" src="https://github.com/user-attachments/assets/81aadcd3-cf49-4f6d-8059-71343c249535" />

### MPG vs Model Year

<img width="508" height="608" alt="image" src="https://github.com/user-attachments/assets/edae74bd-79db-4a94-975d-576981fde455" />

---

## 🔎 Key Insights

The combined statistical analysis and visualizations reveal several important insights:

- MPG decreases as **horsepower increases**, indicating a negative relationship between engine power and fuel efficiency.

- **Vehicle weight shows the strongest negative relationship with MPG**, meaning heavier vehicles tend to consume more fuel.

- **Engine displacement also negatively affects MPG**, suggesting that larger engines generally reduce fuel efficiency.

- **Newer model years tend to have higher MPG**, reflecting improvements in automotive technology and fuel efficiency standards.

Overall, the analysis confirms that **lighter vehicles with smaller engines and newer technology tend to achieve better fuel efficiency.**

## 🛠 Tools Used

- **R Programming (RStudio)** – Performed statistical analysis, exploratory data analysis, and regression modeling to study how automobile engine factors influence MPG.

- **R Libraries (tidyverse, ggplot2, broom, caret)** – Used for data cleaning, visualization, regression modeling, and model evaluation.

- **Tableau** – Created interactive visualizations and dashboard views to explore relationships between MPG and engine characteristics.

- **Auto MPG Dataset** – Used as the primary dataset containing vehicle engine specifications and fuel efficiency data.

- **Statistical Methods** – Linear regression, residual analysis, and exploratory data analysis were used to evaluate relationships between variables.
