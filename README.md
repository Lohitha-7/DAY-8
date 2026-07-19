# DAY-8
DAY 8
# 📊 Day 8 – Data Visualization Using Matplotlib

## 📌 Project Overview

Data visualization is the graphical representation of data that helps users understand trends, patterns, comparisons, and relationships more effectively. Instead of analyzing numbers in tables, visualizations transform data into meaningful charts that make decision-making easier.

In this project, I used the **Matplotlib** library in Python to create three fundamental charts: **Bar Chart**, **Line Chart**, and **Pie Chart**. These visualizations help present the dataset in a clear, interactive, and visually appealing format.

This task demonstrates how graphical representations can simplify data interpretation and support business analytics.

---

# 🎯 Project Objectives

The objectives of this project are:

- Learn the fundamentals of data visualization.
- Create different types of charts using Matplotlib.
- Compare values using a Bar Chart.
- Visualize trends using a Line Chart.
- Display proportions using a Pie Chart.
- Improve data presentation skills.

---

# 🛠 Technologies Used

- 🐍 Python
- 📊 Pandas
- 📈 Matplotlib
- 📒 Jupyter Notebook
- 📄 CSV Dataset

---

# 📂 Dataset Information

The dataset contains student performance records.

### Example Columns

- Student ID
- Name
- Department
- Marks
- Attendance

The **Marks** column is used to create different visualizations.

---

# 📋 Tasks Performed

## ✅ Step 1 – Import Required Libraries

Imported Pandas for data handling and Matplotlib for visualization.

```python
import pandas as pd
import matplotlib.pyplot as plt
```

---

## ✅ Step 2 – Load Dataset

Loaded the CSV dataset into a DataFrame.

```python
data = pd.read_csv("students.csv")
```

---

## ✅ Step 3 – Create a Bar Chart

Created a bar chart to compare student marks.

```python
plt.bar(data["Name"], data["Marks"])
plt.title("Student Marks")
plt.xlabel("Students")
plt.ylabel("Marks")
plt.show()
```

### Purpose

The Bar Chart is useful for comparing values across different categories.

---

## ✅ Step 4 – Create a Line Chart

Created a line chart to visualize student performance.

```python
plt.plot(data["Name"], data["Marks"], marker='o')
plt.title("Student Marks Trend")
plt.xlabel("Students")
plt.ylabel("Marks")
plt.show()
```

### Purpose

The Line Chart helps identify trends and changes in values.

---

## ✅ Step 5 – Create a Pie Chart

Created a pie chart to show the percentage contribution of each student's marks.

```python
plt.pie(data["Marks"], labels=data["Name"], autopct='%1.1f%%')
plt.title("Marks Distribution")
plt.show()
```

### Purpose

The Pie Chart represents the percentage distribution of values.

---

# 💻 Complete Python Program

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load Dataset
data = pd.read_csv("students.csv")

# Bar Chart
plt.figure(figsize=(6,4))
plt.bar(data["Name"], data["Marks"])
plt.title("Student Marks")
plt.xlabel("Students")
plt.ylabel("Marks")
plt.show()

# Line Chart
plt.figure(figsize=(6,4))
plt.plot(data["Name"], data["Marks"], marker='o')
plt.title("Student Marks Trend")
plt.xlabel("Students")
plt.ylabel("Marks")
plt.show()

# Pie Chart
plt.figure(figsize=(6,6))
plt.pie(data["Marks"], labels=data["Name"], autopct='%1.1f%%')
plt.title("Marks Distribution")
plt.show()
```

---

# 📊 Data Visualization Workflow

```
CSV Dataset
      │
      ▼
Load Dataset
      │
      ▼
Read Data
      │
      ▼
Create Bar Chart
      │
      ▼
Create Line Chart
      │
      ▼
Create Pie Chart
      │
      ▼
Visual Analysis
```

---

# 📌 Matplotlib Functions Used

| Function | Purpose |
|----------|---------|
| plt.bar() | Create Bar Chart |
| plt.plot() | Create Line Chart |
| plt.pie() | Create Pie Chart |
| plt.title() | Add Chart Title |
| plt.xlabel() | Label X-axis |
| plt.ylabel() | Label Y-axis |
| plt.figure() | Set Figure Size |
| plt.show() | Display Chart |

---

# 📊 Charts Created

## 📌 Bar Chart

- Compares marks of all students.
- Makes comparison easy.
- Clearly identifies high and low performers.

---

## 📌 Line Chart

- Displays marks as a continuous trend.
- Useful for observing changes and patterns.
- Easy to identify increasing or decreasing values.

---

## 📌 Pie Chart

- Displays percentage contribution of each student's marks.
- Helps understand data distribution.
- Useful for presenting proportional information.

---

# 📈 Expected Outcome

After completing this project:

- Successfully created Bar Chart.
- Successfully created Line Chart.
- Successfully created Pie Chart.
- Visualized data effectively.
- Improved understanding of graphical data representation.

---

# 📊 Business Insights

From the visualizations, the following insights can be observed:

- The Bar Chart quickly identifies the highest and lowest marks.
- The Line Chart shows the variation in student performance.
- The Pie Chart highlights each student's contribution to the total marks.
- Visualizations make complex data easier to understand.
- Charts support better decision-making by presenting information clearly.

---

# 🎯 Learning Outcomes

By completing this project, I learned how to:

- Create charts using Matplotlib.
- Visualize numerical data effectively.
- Compare values using Bar Charts.
- Identify trends using Line Charts.
- Represent proportions using Pie Charts.
- Improve data storytelling through visualizations.

---

# 🚀 Future Scope

This project can be extended by:

- Creating Scatter Plots.
- Developing Histograms.
- Building Box Plots.
- Designing Interactive Dashboards.
- Using Seaborn for advanced visualizations.
- Creating Plotly interactive charts.
- Integrating charts into Power BI or Tableau dashboards.

---

# 📌 Conclusion

Data visualization is an essential component of data analytics because it converts numerical information into meaningful graphical representations. Using Matplotlib, I successfully created Bar Charts, Line Charts, and Pie Charts to analyze and present the dataset effectively. These visualizations improve understanding, simplify decision-making, and communicate insights more clearly.

This project strengthened my practical knowledge of Python, Pandas, and Matplotlib while improving my skills in presenting data visually.

---

# 👩‍💻 Author

**Ketha Lohitha**  
**B.Tech – Data Science**  
**Data Analytics Internship – Day 8**

---

# 🙏 Acknowledgement

I sincerely thank the internship organizers and mentors for providing practical learning opportunities. This task enhanced my understanding of data visualization techniques and helped me develop skills in presenting analytical results through effective graphical representations.
