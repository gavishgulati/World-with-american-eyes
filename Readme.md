# JOUR779V - Computational Journalism Final Project

-----------
Description
-----------

**Data**

Data is in the format of a CSV file where it contains the result for 121 coutries autosuggestions. The data was collected by specifying the domain as Google.com (Domain for US). The next column is Timestamp specifying the time at which the API call was made. The third and last column is the country for which the API call was made. All this data was collected via google autocomplete api. Json Object consists of stereotypes text, country name and stereotype score for each country. Index.html shows the visualization of our analysis on a global map.


---------------
Analysis
---------------

ur analysis of Google autosuggest results for how Americans think about other parts of the world started by collecting data with the help of an API. By parsing through words like “why is Mexico so” as request, we collected Google autosuggest results as our response in a CSV file. SInce our objective was to do the same activity for all the countries in the world (232 countries [1]). After collecting all these countries, we looped through the array of these countries. Many of these countries gave no results at all or gave similar results to their neighbours. Similarity of autosuggest results was prominent amongst countries in Africa. Therefore we discarded these countries and brought down the final number of countries for analysis to 121 countries. We manually went through about 1000 auto suggest results and quantified them to a score between 1 to 5. Each country had an average of 6 to 7 autosuggestions in our dataset. Giving importance to the autosuggest results as per their ranks we gave them higher weightage in our scoring. Results where countries only had one autosuggestion such as “Poor” we assigned it as a score of 3. Our final JSON object which had a list of 121 countries, consisted 4 attributes for each country namely,
Code: This 2 alphabet value helps in mapping the country data to the Highcharts data. Highcharts helps in displaying the map and data such as the flags for each country.
Value: This was the score we assigned to each country based on the sentiment of words collected from Google autosuggest.
Name: Name of the country
Word: List of all the words collected from Google autosuggestion.
We went through the list of words (6800 words) to differentiate positive or negative words which helped us in coming up with the scores for each country
Please visit [Link](http://jour779v.dx.am/) to view the interactive map.
![Interactive Map](https://github.com/gavishgulati/World-with-american-eyes/blob/master/World-With-American-Eyes.JPG)

-----
Files
-----

*google autosuggest data.csv*

*stereotype-data.json*

*index.html* (Please place the JSON file and this HTML file in the same directory to see the interactive map.)

*Autosuggest_collect.py.ipynb*


----------------
Acknowledgements
----------------

   We thank Dr. Diakopoulos for the ideas and guidance.

----------
References
----------

	www.statvision.com/webinars/countries%20of%20the%20world.xls

	Hu, M., & Liu, B. (2004, August). Mining and summarizing customer reviews. In Proceedings of the tenth ACM SIGKDD international conference on Knowledge discovery and data mining (pp. 168-177). ACM.

-------
Author
-------

Gavish Gulati.

Emily Goldman
