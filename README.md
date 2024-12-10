
_**Data-driven custom Airbnb Pricing Analysis - Using ML to create better listings**_

**PRICING RECOMMENDATION FOR NEW LISTINGS**

Extending Insights to New Listings: Take listing information as input from the host.

Cluster Assignment: Assigned new listings to established clusters utilizing the K-means model - The model can adapt to diverse input listing data

Pricing Recommendation: Get the median price of the assigned cluster, suggest a price range for the new listing +- 12.5% of the median price

_Pricing Recommendation Calculations:_

Recommending a range of prices to be set depending on the Neighborhood, Room type, Minimum number of nights and host listings. A price range of ± 12.5% is recommended to include a buffer for providing discounts and breaking into the competitive market. Host pays a flat 3% (incl cleaning fee) service fee to Airbnb per booking. Customers pay a 14% service fee to Airbnb per booking.

**KEYWORD RECOMMENDATION FOR LISTING NAME**

Technique: Text Mining

Features: Listing Name

Modeling and Solution Delivery: Clean, pre-process, tokenize and vectorize listing names. Calculate the median reviews for existing listings in the assigned cluster. Use the median threshold as a filter to retrieve all listings in the assigned cluster that exceed the threshold

Filters applied: Cluster assigned, Median reviews threshold

Keyword Recommendation: Extract frequently used keywords from these listing names. Recommend the top 20 popular keywords to host for the new listing name.

**Data Source:**

https://www.kaggle.com/datasets/kritikseth/us-airbnb-open-data?select=AB_US_2023.csv
