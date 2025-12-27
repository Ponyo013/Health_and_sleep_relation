<h1>Health and Sleep Correlation Test</h1>
<p>The data set is provided by: ORVILE<br>Source: https://www.kaggle.com/datasets/orvile/health-and-sleep-relation-2024</p>

<h2>Data Transformation</h2>
<p>
  Before going into the result explanation, there are some data transformation
  processes that need to be done, including:
</p>
<ol>
  <li>
    Changing NaN values to <code>None</code> in the <strong>Sleep Disorder</strong> column
  </li>
  <li>
    Applying Label Encoding to columns with categorical values
    (e.g. <strong>Sleep Disorder</strong>, <strong>BMI Category</strong>, etc.)
  </li>
  <li>
    Splitting the <strong>Blood Pressure</strong> column into two separate columns:
    <strong>Systolic</strong> and <strong>Diastolic</strong>
  </li>
  <li>
    Dropping unused columns such as <strong>Blood Pressure</strong>
    (since it is replaced by the separated values) and <strong>Person ID</strong>
  </li>
</ol>

<h2>Correlation Test Result</h2>
<p>
  Correlation coefficient (r) measures the strength and direction of a linear relationship between two variables, ranging from -1 (perfect negative) to +1 (perfect positive), with 0 meaning no correlation
  <br><br>
  <img width="676" height="558" alt="download" src="https://github.com/user-attachments/assets/5e841b44-a346-43b8-9c18-8e09ab1e46ca" />
  <br><br>
  The following heatmap shows a few key points:
  <ol>
    <li>
      Sleep duration shows a weak to moderate positive correlation with age (r = 0.34), 
      indicating that older age groups tend to have slightly longer sleep durations.
    </li>
    <li>
      Sleep quality is strongly positively correlated with sleep duration (r = 0.88). 
      This suggests that longer sleep duration is closely associated with better sleep quality.
    </li>
    <li>
      Both systolic and diastolic blood pressure exhibit moderate positive correlations with age (r = 0.61 and r = 0.59, respectively).
      This implies that blood pressure levels tend to increase as age increases.
    </li>
    <li>
      Stress level has a strong negative correlation with sleep quality (r = −0.90), 
      indicating that higher stress levels are associated with poorer sleep quality.
    </li>
    <li>
      Daily steps show a strong positive correlation with physical activity level (r = 0.77), 
      suggesting that individuals with higher step counts generally engage in higher levels of physical activity.
    </li>
  </ol>
</p>

<h2>Closing</h2>
<p>
  This test is conducted for learning purpose only. Especially in learning to perform a correlation test and data transformation on raw data.
</p>
