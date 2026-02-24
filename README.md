# Wine-Quality-Analysis-PowerBI
Interactive Power BI dashboard analyzing 6,497 wine records to identify quality-driving factors.
To analyze wine quality based on chemical properties and build an interactive Power BI dashboard that provides business insights for quality optimization.

Dataset: Wine Quality Dataset (Red Wine & White wine)

-Features include:
Fixed Acidity
Volatile Acidity
Citric Acid
Residual Sugar
Chlorides
Free Sulfur Dioxide
Total Sulfur Dioxide
Density
pH
Sulphates
Alcohol
Quality (Target Variable)

-Tools & Technologies
Power BI Desktop
Power Query (Data Cleaning)
DAX (Data Modeling & Measures)

-Data Preparation Steps
1.Imported CSV dataset into Power BI.
2.Verified data types in Power Query.
3.Removed null values and duplicates.
4.Renamed columns for clarity.

-Created Quality Category column:
Low (≤5)
Medium (6)
High (≥7)

-DAX Measures Created
Total Wines = COUNT(Wine[quality])
Average Alcohol = AVERAGE(Wine[alcohol])
Average Quality = AVERAGE(Wine[quality])

Low Quality Wines = 
CALCULATE(
    COUNT(Wine[quality]),
    Wine[quality] <= 5
)

High Quality Wines = 
CALCULATE(
    COUNT(Wine[quality]),
    Wine[quality] >= 7
)

-Dashboard Features
1.KPI Cards (Total Wines, Avg Alcohol, Avg Quality)
2.Alcohol vs Quality Analysis
3.Citric Acid Trend Analysis
4.Wine Type Distribution (Donut Chart)
5.Quality Category Comparison
6.Interactive Wine Type Slicer

-Key Insights
1.Alcohol positively impacts wine quality.
2.Higher citric acid levels are observed in high-quality wines.
3.Most wines fall in medium quality range.
4.White wines represent majority of dataset (~75%).

-Business Impact
1.Helps optimize chemical composition.
2.Supports data-driven production decisions.
3.Identifies improvement areas for low-quality wines.
4.Enables focus on premium wine segment.

