# Data-harvesting
To harvest brownfield data from a public source. Please write a python harvester in class abstraction and scalable manner (Object Oriented Programming). The output should be tabular, cleanly structured data (.csv or .json), preferably with data for 500-1000 samples. 


I used Beautiful Soup 4 for the scraping and I decided to go with one of the URLs given in the problem statement.

After extracting all the html content I used find_all from the bs4 library to collect all the table row entries in the website as they were all entered using the tr tag.
Made a seperate list of the table headings, used find_all for that as well, and looked for the th tagged in the html content.
Every row had the data entered in it with the tags td, used a simple for loop and find all to extract that.

A simple for loop while we write using DictWriter to make the final csv.


url_used : Solar -- https://list.solar/plants/largest-plants/largest-pv-plants/ 
