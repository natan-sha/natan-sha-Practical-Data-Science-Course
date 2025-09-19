# Week 3: Data Visualization with Plotly

## 📚 Overview

Learn to create compelling, interactive visualizations that tell stories about social issues. This week focuses on using Plotly to transform data into clear, engaging charts that communicate insights effectively.

## 🎯 Learning Objectives

By the end of this week, you will be able to:

- Understand why visualization matters for social impact storytelling
- Create interactive charts using Plotly (scatter, bar, line, box plots)
- Choose appropriate chart types for different data and questions
- Add proper titles, labels, and styling to make charts publication-ready
- Build visualizations that reveal patterns and insights in social data
- Export and share interactive charts

## 🎓 Session Structure (80 minutes)

### Lecture (40 minutes): Why Visualization Matters for Storytelling

**Topics Covered:**
- The power of visual communication for social change
- Chart types and when to use them:
  - **Scatter plots**: Relationships between variables
  - **Bar charts**: Comparisons across categories  
  - **Line charts**: Trends over time
  - **Box plots**: Distribution and outliers
- Design principles: clarity, honesty, accessibility
- Interactive features that enhance understanding

### Tutorial (40 minutes): Creating Interactive Charts

**Hands-on Activities:**
- Create a scatter plot showing relationship between education and health outcomes
- Build a bar chart comparing progress across countries
- Design a line chart showing trends in social indicators over time
- Add interactive features: hover information, zoom, selection
- Style charts with appropriate colors, titles, and labels

## 🏗️ Mini-Deliverable

**Assignment:** Create at least one polished Plotly chart with titles and labels that tells a story about a social issue.

**Requirements:**
1. **Choose a social dataset** (education, health, environment, etc.)
2. **Create 2-3 different chart types** that answer specific questions
3. **Add interactive features** (hover info, zoom, filtering)
4. **Include proper styling** (titles, axis labels, colors, legends)
5. **Write brief interpretations** explaining what each chart reveals
6. **Export charts** as HTML files for sharing

### Example Visualization Goals:
```python
import plotly.express as px
import pandas as pd

# Load your social impact dataset
df = pd.read_csv('global_education_data.csv')

# 1. Scatter plot: Education spending vs. literacy rates
fig1 = px.scatter(df, 
                  x='education_spending_per_capita', 
                  y='literacy_rate',
                  color='region',
                  size='population',
                  hover_name='country',
                  title='Education Spending vs. Literacy Rates by Region')
fig1.show()

# 2. Bar chart: Top 10 countries by gender education gap
education_gap = df.nlargest(10, 'gender_education_gap')
fig2 = px.bar(education_gap, 
              x='country', 
              y='gender_education_gap',
              title='Countries with Largest Gender Education Gaps')
fig2.show()

# 3. Line chart: Literacy trends over time
fig3 = px.line(df, 
               x='year', 
               y='literacy_rate', 
               color='income_level',
               title='Global Literacy Rate Trends by Income Level')
fig3.show()
```

## 📁 Files Structure

```
week3/
├── README.md
├── notebooks/
│   ├── lecture_visualization_principles.ipynb
│   ├── tutorial_plotly_basics.ipynb
│   └── assignment_story_charts.ipynb
├── charts/
│   ├── interactive_exports/
│   └── static_examples/
├── data/
│   ├── education_indicators.csv
│   ├── health_outcomes.csv
│   └── climate_data.csv
└── resources/
    ├── plotly_cheatsheet.md
    ├── color_palettes.md
    └── chart_design_guide.md
```

## 📖 Key Concepts Introduced

### Plotly Fundamentals
- **Interactive charts**: Users can zoom, hover, filter
- **Express vs. Graph Objects**: Simple vs. detailed control
- **Chart types**: Each tells a different story
- **Styling**: Colors, fonts, layout customization

### Essential Plotly Patterns
```python
import plotly.express as px

# Scatter plot for relationships
px.scatter(df, x='variable1', y='variable2', color='category')

# Bar chart for comparisons
px.bar(df, x='category', y='value', title='Chart Title')

# Line chart for trends
px.line(df, x='time', y='value', color='group')

# Box plot for distributions
px.box(df, x='category', y='value')

# Add interactivity
fig.update_layout(
    title='Clear, Descriptive Title',
    xaxis_title='X Axis Label',
    yaxis_title='Y Axis Label'
)
```

### Design Principles for Social Impact
- **Clarity**: Charts should be immediately understandable
- **Honesty**: Don't mislead with scale or visualization choice
- **Accessibility**: Consider colorblind-friendly palettes
- **Context**: Always explain what the data shows and why it matters

## � Video Resources

1. **The Power of Data Visualization for Social Change** (15 min)
2. **Plotly Basics: Your First Interactive Chart** (20 min)
3. **Choosing the Right Chart Type** (15 min)
4. **Styling and Polish for Professional Charts** (10 min)

## 📊 Visualization Project Ideas

Choose one area that interests you:

### Education Equity
- Literacy rates vs. economic development
- Gender gaps in education across regions
- School enrollment trends over time
- Education spending effectiveness

### Global Health
- Life expectancy vs. healthcare spending
- Disease prevalence by income level
- Vaccination coverage progress
- Maternal mortality trends

### Climate & Environment
- Temperature changes over time by region
- CO2 emissions vs. economic development
- Renewable energy adoption rates
- Extreme weather event frequency

### Economic Development
- Income inequality trends
- Poverty reduction progress
- Economic growth vs. social outcomes
- Access to basic services

## 🎨 Chart Type Guide

### When to Use Each Chart Type

**Scatter Plots** 📈
- Exploring relationships between two continuous variables
- Looking for correlations or patterns
- Example: GDP per capita vs. life expectancy

**Bar Charts** 📊
- Comparing values across categories
- Showing rankings or top/bottom performers
- Example: Literacy rates by country

**Line Charts** 📉
- Showing trends over time
- Comparing multiple groups' progress
- Example: Poverty rates from 1990-2020

**Box Plots** 📦
- Understanding data distributions
- Identifying outliers
- Example: Income distribution by region

## 🔗 Additional Resources

### Plotly Documentation
- [Plotly Express Guide](https://plotly.com/python/plotly-express/)
- [Plotly Color Scales](https://plotly.com/python/colorscales/)
- [Interactive Features](https://plotly.com/python/interactive-html-export/)

### Data Visualization Inspiration
- [Our World in Data Charts](https://ourworldindata.org/)
- [Gapminder Visualizations](https://www.gapminder.org/tools/)
- [Hans Rosling TED Talks](https://www.ted.com/speakers/hans_rosling)

### Design Resources
- [Data Visualization Catalogue](https://datavizcatalogue.com/)
- [ColorBrewer 2.0](https://colorbrewer2.org/)
- [Accessibility Guidelines](https://accessibility.digital.gov/visual-design/color-and-contrast/)

## ❓ Common Questions

**Q: My charts look boring. How can I make them more engaging?**
A: Focus on storytelling! Add meaningful titles, use color strategically, and include context about why the data matters.

**Q: Should I always use interactive charts?**
A: Interactive features are great when they add value (like exploring different countries), but don't add complexity just for the sake of it.

**Q: How do I choose colors for my charts?**
A: Use colorblind-friendly palettes, ensure sufficient contrast, and consider cultural associations (red often means danger/bad).

**Q: My dataset is huge. Should I plot everything?**
A: No! Filter to the most relevant data or use sampling. A clear chart with 20 countries is better than a cluttered one with 200.

## 🆘 Getting Help

- **Discussion Forum**: Share charts for feedback
- **Office Hours**: Tuesdays 6-7 PM
- **AI Assistants**: Great for Plotly syntax questions
- **Peer Support**: Exchange datasets and chart ideas

## 📈 Assessment Criteria

Your visualization assignment will be evaluated on:
- **Technical Execution**: Charts render correctly with proper syntax
- **Design Quality**: Clear titles, labels, appropriate colors and styling
- **Chart Selection**: Appropriate chart types for the data and questions
- **Storytelling**: Visualizations reveal insights about social issues
- **Interactivity**: Meaningful use of hover, zoom, or filtering features

---

**Next Week**: [Week 4: Organizing Projects with GitHub + First Encounter with AI Helpers](../week4/README.md)

**Previous Week**: [Week 2: Working with DataFrames (Pandas Basics)](../week2/README.md)
