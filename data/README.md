This file describes the purpose of the datasets in this directory and notes what the data in each column represents.

341379231_T_MASTER_CORD.csv
The Bureau of Transportation Statistics provides data on a 10% sample of flights and airline tickets going back to 1993 and recorded quarterly. The data can be filtered by destination airport and date. Bay Area destination airports of interest to us are San Francisco International Airport and Oakland International Airport. 
***DB1BMarket***
- ItinID (int): a unique itinerary identifier which will help us connect the two tables together
- Orig and Dest (string): three letter airport codes for the origin/destination airport
- OriginAirportID(int) and DestAirportID (int): a unique identifier for the origin/destination airport
- Year and Quarter (string and int)
- Passengers (int): number of passengers

***DB1BTicket***
- ItinID (int): a unique itinerary identifier which will help us connect the two tables together
- RoundTrip (int): a round trip indicator (1=Yes, 0=No)
- ItinFare and FarePerMile (float): fares for the entire itinerary and per mile flown, respectively



BA_AQI_STATIONS.csv
This dataset has info about the Site where the Air data was collected. Its contains location and dates of operation data.



BA_AQI_STATIONS.json
This dataset has info about the Site where the Air data was collected. Its contains location and dates of operation data. (but in a json format)



BA_County_Data.json
This dataset has info about each county in the Bay Area (BA).



BA_ZIP_CODES.csv
This dataset has info about each ZIP code in the Bay Area.



California_Fire_Incidents.csv
- Counties (string): counties in which the fire was active
- Started (string): date the fire started
- Extinguished (string): date the fire was extinguished
- Latitude and Longitude (float)


Final_Listings.csv
This is the AirBnB Listing data. It will be used in conjunction with our AirBnB Bookings Calendar dataset
1. *id*: The unique identifier of the Airbnb listing
1. *name*: The name of the listing
2. *host_id*: A unique identifier of the Airbnb host
3. *host_name*: The host's name
4. *neighbourhood_group*: A blank column
5. *neighbourhood*: Name of the listing's neighbourhood
5. *latitude*: Latitude of the listing
6. *longitude*: Longitude of the listing
6. *room_type*: Type of room of the listing
7. *price*: Price for a day of the listing
8. *minimum_nights*: Minimum required nights for booking
9. *number_of_reviews*: The number of reviews the listing has
10. *last_review*: Date of the last review
11. *reviews_per_month*: Ratio of reviews/ month since the listing was added
12. *calculated_host_listings_count*: The amount of listings the host has in total
13. *availability_365*: The amount of days the listing is available for in the next 365 days

Calendar Dataset
1. listing_id: The unique identifier of the Airbnb listing. 
2. date: The date of interest
3. available: Availability of the listing for the specific date, in which *t* = available and *f* = not available.
4. price: Price of the listing.



Max_PM25.csv
This file contians the data for the Air Quality Index.
https://aqs.epa.gov/aqsweb/airdata/FileFormats.html
3. county_code: The FIPS code of the county in which the monitor resides.The numeric code for the county where the reading was observed
4. site_number: A unique number within the county identifying the site.
7. latitude: The monitoring site’s angular distance north of the equator measured in decimal degrees.
8. longitude: The monitoring site’s angular distance east of the prime meridian measured in decimal degrees.
13. date_local: The calendar date for the summary. All daily summaries are for the local standard day (midnight to midnight) at the monitor.
19. arithmetic_mean: The average (arithmetic mean) value for the day.
20. first_max_value: The highest value for the day.
21. first_max_hour: The hour (on a 24-hour clock) when the highest value for the day (the previous field) was taken.
25. local_site_name: The name of the site (if any) given by the State, local, or tribal air pollution control agency that operates it.
26. site_address: The approximate street address of the monitoring site.
28. county: The name of the county where the monitoring site is located.
29. city: The name of the city where the monitoring site is located. This represents the legal incorporated boundaries of cities and not urban areas.

