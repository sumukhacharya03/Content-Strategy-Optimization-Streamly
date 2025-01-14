# Content-Strategy-Optimization-Streamly

## About the Project:
In the world of streaming services, optimizing content strategy is crucial for attracting and retaining users. Companies like Streamly are constantly striving to understand what content resonates most with their audience, how to improve user engagement, and how to forecast trends to stay ahead of the competition.

Streamly has a rich dataset containing information about movies and series' aired on the platform. I analysed the data and provide valuable insights that can guide Streamly's decision-making.

## Evaluation Metric:
**R-Squared (R²)**

The R-Squared value is calculated as:
```python
from sklearn.metrics import r2_score

r2 = r2_score(y_test, predict)
print(f'R-squared: {r2}')

```

Higher the R-square value, the better the fit and closer the model's predictions are to the actual outcomes.


## Methodology Used:

1. **Data Exploration and Preparation**:
   - Checked for null values and duplicate rows.
   - Performed encoding of categorical columns.
   - Checked for outliers using the BoxPlot and capped the outliers to keep them within a reasonable range.

2. **Comprehensive Movie Performance Analysis**:
   - Plotted correlogram to visualize the relationships between all numerical variables.
   - Then found out ROI(Return on Investment) and EAROI across different movie genres, and plotted it using barplot to visualize it.
   - Compared ROI and EAROI using histogram.

3. **Correlation analysis**:
   - Applied log on user_retention to limit it to range of 0-100.
   - Plotted correlogram heatmap and drew inferences from these to improve user retention.

4. **User Retention Analysis and Modeling**:
   - Analyzed how each feature affects user retention.
   - Applied models MLR(Mutiple Linear Regression) and RFR(Random Forest Regressor).
   - Tested the Model for the Test Dataset.
