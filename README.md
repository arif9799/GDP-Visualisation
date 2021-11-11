# GDP-Visualisation
Visualizing GDP trends (with peaks) for various countries for the last 6 decades          
Used the WDI Package to pull GDP data of the last 60 years for certain specific countries using the WDI Function. 
WDI Package contains region wise and year wise (in row fashion) and all the development indicators (in column fashion). 
The data was pulled using its WDI function, wherein the frame of the subset of data can be fetched by mentioning the years 
and region for the rows and some specifically coded indicators which is listed on the official website of world bank. 

It also has a WDI Search function, which is used to cluster indicators based on similar factors.
For example, if you search for mortality rates, all those indicators related to mortality: whether male or female or mixed 
or youth or old age etc., that come under the mortality data.

After pulling the GDP data for certain selected countries (subset of 60 years), the data was plotted using the library named ggplot2 
and scales (used by ggplot2 for internal scaling and more extended features of data points)

The indicators pulled for GDP from WDI are NY.GDP.PCAP.CD, NY.GDP.MKTP.CD which is GDP per capita and Annual GDP respectively.
The plots are for GDP per Capita and Annual GDP (Single Graph with multiple geom smooth lines and faceted region wise or country wise) 
