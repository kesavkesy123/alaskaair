# alaskaair

1.	What is the conversion rate for an individual flight search result? For definition, an ‘individual flight search result’ is the following:
 
- Develop a Dataset based on flight search portal at alaskaair.com. Different attributes can be deducted. The attributes can be Search index, from location, To location, Departure date, Return date, Number of adults, number of children, One way (yes/no), cost in miles(yes/no), Flight available(yes/no), Flight number, Payment done(yes/no), Flight Fare.
- Each time the individual searches for a flight, the values are recorded in the database. Only after the payment is done, the payment done column will update as ‘Yes’ otherwise ‘No’.  
-The individual flight search result can be identified using the percentage difference of the total payment done (yes) count to the total number of search index. 
-This index can be shown using data visualization techniques likes chart or a graph or in percentage value. 


2.	How does the cost in miles affect the guests’ willingness to purchase? For this question, assume that the conversion space is already tagged successfully, and this data is already accessible.

 --> Assuming that the conversion space is already tagged successfully, and this data is already accessible, the cost in miles column will update as ‘YES’ if the customer has chosen the cost in miles payment method otherwise ’NO’. 

--> Based on this index taking the count of ‘YES’ against the total number of conversions we can get the percentage of customers that has chosen the cost in miles payment method. 

--> The outcome can be displayed using Data visualization techniques like charts or graphs or in percentage value. Based on this index, we can have an assumption whether the cost in miles payment method has benefited the customers.

3.	How many times does a guest attempt to search for a destination that we do not serve for the given airport or date? This can be demoed through the following flight search: And provide model for recommendation to guest on what itenary would be helpful for guest and will generate revenue.

--> Assuming we already have a Scheduled Flight Database having details like From location, To location, Date, Flight Number, No of seats available, Standard Fare, Percentage discount available etc.

--> Soon after the customer searches for a flight, the search details will be stored in our Individual search result database. 

--> This search result should cross check with the Scheduled Flight database and the result is updated as ‘Yes’ if the Flight is available, otherwise ‘No’ on the Flight Availability column in the Individual search result database. 

--> Based on this result, the ‘No’ result can be counted to know the index of failed customer search.
The result can be displayed as count or percentage against the total search or as charts or graphs. 
--> Content based Recommendation algorithm can be used to generate a recommended Scheduled Flights list for the customers for seeking possible Flight booking. The attributes like Date, from location, To location, Flight Fare, Percentage of discount available can be used as parameters on the Recommendation algorithm. 
--> The attributes can be altered according to the company priority.

--> The Datasets can be handled in JSON format. 
--> The Data Visualization can be developed using 3rd party applications like Power BI, Tableau.
-->	The Various charts can be displayed on the company website, so that the customer can understand the usage index of the company. 

	Pros: If the conversion rate is more the customer impression will be positive and chance to get converted will be more.
	Cons: If the conversion rate is less, the customer will get negative impression.

-->	The Scheduled Flight database having scheduled flight details like from location, To location, Flight number, Flight Fare, Number of seats available, Percentage of discount available etc., and The Individual Search Index Result database can be stored in Cloud storage platforms like Microsoft Azure Storage. The data can be stored in SQL format. These data can be used in our model using storage handling technologies like Spark and can be converted to Pandas Data frame. Other Modelling, programming and operations like Recommendation engine can be done after that.





