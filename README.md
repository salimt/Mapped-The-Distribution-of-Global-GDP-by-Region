# GDP-Data-Visualization-on-World-Map
_this was the final homework for Rice University's Python Data Visualization._

My approach was to link Pygal's map dictionary (mapping 2-letter country codes to country names) to a dictionary that stored World Bank GDP country data keyed by the **"Country Name"** field.

This approach worked modestly well, but left part of the resulting world map blank with no plotted GDP data. In many of these cases, the missing data was due to slight differences in how a country's name was represented in Pygal vs. the World Bank data set. For example, the country name **"Viet Nam"** in pygal corresponds to the country name **"Vietnam"** in the World Bank data.

An alternative approach would be to use the three-letter **"CountryCode"** in the World Bank data set to reconcile Pygal's country information with the World Bank's country information. In this case, we will need to determine how to map Pygal's two-letter country codes (e.g. **"vn"** for Vietnam) to the World Bank's three-letter country codes (e.g **"VNM"** for Vietnam).

> ### **Example for 2010:**

 <a><img src="https://storage.googleapis.com/codeskulptor-isp/course4/isp_gdp_world_code_2010.svg"/></a> 
