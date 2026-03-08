
# R-Tableau-auto-mpg-trends-analysis

This project analyzes how automobile engine characteristics influence fuel efficiency (MPG) using statistical analysis in R and data visualization in Tableau. The workflow begins with statistical exploration and regression analysis in R, followed by visual exploration and dashboard creation in Tableau to communicate insights effectively.

---

## 1️⃣ Statistical Analysis using R

The first stage of this project involved performing statistical analysis in R to understand how engine-related factors impact vehicle fuel efficiency (MPG).

Using the Auto MPG dataset, several engine characteristics were examined, including:

- Horsepower  
- Weight  
- Displacement  
- Cylinders  
- Model Year  
- Origin  

### Data Preparation

Before conducting statistical analysis, the dataset required preprocessing:

- The **horsepower column contained missing values represented as "?"**
- Horsepower values were **converted to numeric format**
- Missing horsepower values were **replaced using the median** to reduce the effect of outliers

### Statistical Analysis in R

Using R, the following analytical steps were performed:

- Exploratory data analysis of the Auto MPG dataset  
- Summary statistics of engine variables  
- Linear regression analysis to examine how engine factors influence MPG  
- Evaluation of relationships between MPG and variables such as horsepower, weight, displacement, cylinders, and model year  

These statistical results provided an analytical understanding of which engine characteristics most strongly influence fuel efficiency.

---

## 📊 Statistical Outputs (R)

Below are selected outputs from the statistical analysis performed in R.

### Regression Output

<img width="900" alt="Regression Output" src="ADD_R_SCREENSHOT_1">

### Statistical Summary

<img width="900" alt="Statistical Summary" src="ADD_R_SCREENSHOT_2">

### Additional Statistical Results

<img width="900" alt="R Analysis Output" src="ADD_R_SCREENSHOT_3">

---

## 2️⃣ Data Visualization using Tableau

After completing statistical analysis in R, the dataset was visualized using Tableau to better understand and communicate the relationships between engine characteristics and MPG.

Interactive scatter plots were created to visually explore how different variables influence fuel efficiency.

### Visualizations Created

The following visualizations were developed in Tableau:

- Scatter Plot: MPG vs Horsepower  
- Scatter Plot: MPG vs Weight  
- Scatter Plot: MPG vs Displacement  
- Scatter Plot: MPG vs Model Year  

These visualizations help clearly reveal patterns between engine features and fuel efficiency.

---

## 📊 Tableau Visualizations

### MPG vs Horsepower

<img width="900" alt="MPG vs Horsepower" src="ADD_TABLEAU_IMAGE_1">

### MPG vs Weight

<img width="900" alt="MPG vs Weight" src="ADD_TABLEAU_IMAGE_2">

### MPG vs Displacement

<img width="900" alt="MPG vs Displacement" src="ADD_TABLEAU_IMAGE_3">

### MPG vs Model Year

<img width="900" alt="MPG vs Model Year" src="ADD_TABLEAU_IMAGE_4">

---

## 🔎 Key Insights

The combined statistical analysis and visualizations reveal several important insights:

- MPG decreases as **horsepower increases**, indicating a negative relationship between engine power and fuel efficiency.

- **Vehicle weight shows the strongest negative relationship with MPG**, meaning heavier vehicles tend to consume more fuel.

- **Engine displacement also negatively affects MPG**, suggesting that larger engines generally reduce fuel efficiency.

- **Newer model years tend to have higher MPG**, reflecting improvements in automotive technology and fuel efficiency standards.

Overall, the analysis confirms that **lighter vehicles with smaller engines and newer technology tend to achieve better fuel efficiency.**
