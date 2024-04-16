# Geo-Map-of-Finnish-Metal-Bands
![immagine](https://user-images.githubusercontent.com/45571791/236247325-826bcd49-e39a-42c4-878e-c1f31e6b6c28.png)


A simple and funny project with GeoPandas and Selenium.

Goal: Download data from online Metal bands archive and create a dataframe. Then, after analyzed and properly managed, I merged these info with other geojson files in order to make static/interactive map visualization with GeoPandas and Plotly

UPDATE (APRIL 2024): I uploaded an updated version of my file (now called "Project3_Geo_NEW"). It just changes the very first lines of code due to:
-  Selenium new versions (from 4.6 onwards) don't need to specify services for webdrivers
- After the introduction of safety measures in " www.metal-archives.com" and the "Verify you're human" button, I add to ask for a temporary permission (user agent) to retrieve data. As this "key" will not be displayed for safety measures, you won't be able to download data using the very first lines of code. However, I managed to save these data into an excel file ("Finnish_bands2.xlsx") so that you can run the code from the line:
   fin_bands=pd.read_excel("Finnish_bands2.xlsx",index_col=0)
