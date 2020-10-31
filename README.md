### Pyviz_Homework
### Student: Michael De Paula


---
---

<p align="center">
    <ins><b>Pyviz Visualization:</b><br><ins>
    
</p>

The code in this repository represents the housing market in San Francisco from 2010 - 2016.
We will be coding a sales price and rental analysis per neighborhood in a jupyter file by the name of rental_analysis and we will be visualizing the analysis in a panel dashboard in a jupyter file by the name of dashboard.


The following imports will be used to create each file of code:
- import os
- import pandas as pd
- import panel as pn
- from panel.interact import interact
- from panel import widgets
- import matplotlib.pyplot as plt
- import plotly.express as px
- import hvplot.pandas
- from pathlib import Path
- from dotenv import load_dotenv
- %matplotlib inline
- load_dotenv()
- mapbox_token 
- px.set_mapbox_access_token()
- pn.extension()


In order to begin the analysis we will pull CSV file sfo_data already saved in the Data folder and convert them to dataframes. Once converted we will use Pandas, plotly, hvplot and pyplot to calculate and plot the mean, average gross rent, average sales price per year, average prices by neighborhood. We will then adjust the dataframe to reflect the top 10 most expensive neighborhoods. We will use a basic bar plot to visualize the Top 10 data and then create a parallel coordinate and parallel categories analysis to compare the data in the Top 10 dataframe. We will then use the same sfo_data file to combine it with another CSV file, neighborhood_coordinates and plot the data on a Map. In order to do this we will use Mapbox as a scatter plot. 

Finally, using the jupyter file dashboard we will combine all the visualizations created in the rental_analysis to create a panel dashboard. In order to create this panel we have to define each vizualization as a function and call them using the pn.Column or pn.Row function witin pn.Tabs. This visualization will also be visible via a webapp using the .servable() function. With this function typing the following in a terminal screen you will be able to visualize the data on a webpage:  
- panel serve FILE_NAME.ipynb --log-level debug --show

## Enjoy!  

