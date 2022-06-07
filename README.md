# Exploratory-Data-Analysis-AirBnB

### **Business Problem Understanding**

#### Context

AirBnB is an online marketplace platform for people who wants to rent their property either as a hotel room, hostel, even an entire home/property such as villa even their own home/property. The interaction that occurs in AirBnB is AirBnB as a two sided platform or the third party where the host who wants to rent their property submit their property, set the price, accepted and it will be in the AirBnB platform. The visitor who need an accomodation will find what they need in AirBnB, book it from AirBnB application and contact the host.

![airbnb](https://user-images.githubusercontent.com/99155979/172291898-8f985b76-3294-4492-b21c-f2aa17099682.jpg)

[Image Source](https://bmtoolbox.net/stories/airbnb/)

AirBnB has been operating since 2008 and has covered more than 150 country around the world. Based on [New York City planning](https://www1.nyc.gov/site/planning/planning-level/nyc-population/population-facts.page), New york city as one of the most populated city in USA has been taking part for the growth of AirBnB Business, which is a lot of tourist need an accomodation to stay.

#### Problem Statement

One of the issue is how the host able to set the suitable price within others similar type of property and within the areas, that's because Airbnb offers hosts a complete freedom to set the price for their own property, providing only minimal clues that allow hosts to compare similar places in their neighborhood for competitive prices.

#### Goals

From the issue, Air BnB needs to make an analysis based on the demographics what kind of prperty most of people rent and which area and neighborhood a lot of people rent, so AirBnB can support client to set the suitable price.


## 2. Data Understanding

**Attributes Information**

| **Attribute** | **Data Type** | **Description** |
| --- | --- | --- |
| id | Integer | Listing ID |
| name | Object | Name of the listing |
| host_id | Integer | Host ID |
| host_name | Object | Name of the host |
| neighbourhood_group | Object | Location |
| neighbourhood | Object | Area |
| latitude | Float | Latitude coordinates |
| longitude | Float | Longitude coordinates |
| room_type | Object | Listing space type |
| price | Integer | Price in dollars |
| minimum_nights | Integer | Amount of nights minimum |
| number_of_reviews | Integer | Number of reviews |
| last_review | Object | Latest review |
| reviews_per_month | Float | Number of reviews per month |
| calculated_host_listings_count | Integer | Amount of listing per host |
| availability_365 | Integer | Number of days when listing is available for booking |

<br>

## 3. Data Preprocessing

<img width="505" alt="image" src="https://user-images.githubusercontent.com/99155979/172290858-d0d39a93-c6d0-4d1e-837d-b88e0b0eecef.png">
==========================================================================

```python
There are four features with missing value. which is 'last_review' dan 'reviews_per_month' with the same amount of missing value 
with almost 21% from total data, the other two is feature 'name' and 'host_name' this two feature will not be used so we are 
going to drop this four feature
```

<img width="572" alt="image" src="https://user-images.githubusercontent.com/99155979/172291045-499858ca-878d-45ab-97b2-3d762198ba7c.png">
==========================================================================
<img width="419" alt="image" src="https://user-images.githubusercontent.com/99155979/172291116-9828dd09-6805-4ec1-abd8-c53c78f55fda.png">
==========================================================================
<img width="385" alt="image" src="https://user-images.githubusercontent.com/99155979/172291154-540a83c7-925c-4cd6-a08d-72e9b297c19a.png">
==========================================================================

```python
The rest missing value come from feature the last review. After analyzing it, the missing value is from the old data that before
a specific time and at the same time to make the data exaclty 8 years by the timestamp
```

<img width="338" alt="image" src="https://user-images.githubusercontent.com/99155979/172291199-38d5a3af-3deb-4cb3-9e18-93b996ec674e.png">
==========================================================================

```python
The data with 0 value in price is also will be dropped.
```

<img width="398" alt="image" src="https://user-images.githubusercontent.com/99155979/172291839-19bef1a1-c6e3-4852-be03-829c21bc0ae0.png">
==========================================================================
<img width="392" alt="image" src="https://user-images.githubusercontent.com/99155979/172292112-86b79acd-c213-4ce8-a427-d9c8add50399.png">



