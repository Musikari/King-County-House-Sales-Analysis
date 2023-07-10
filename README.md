# King-County-House-Sales-Analysis

Business and Data Understanding
Explain your stakeholder audience here
Modeling
Regression Results
Conclusion
## OVERVIEW
King County is located in the U.S. state of Washington. It is the most populous county in Washington and the 13th-most populous in the United States. The county seat is Seattle, also the state's most populous city.

## Business Understanding
A real estate agent of a company in Seattle(stakeholder) wants to know which factors significantly impact the prices of a house in King County. This will aid in strategizing the best criteria to take in order to maximize profit. I have been given the task by the company to come up with a model that will be used to predict property prices in King County and obtain significant recommendations on steps that they should take for the business to be successful.

Stakeholders:

The Real Estate Agents who are the stakeholders play an important role between homeowners who are willing to sell their houses and potential buyers. They are responsible for listing and marketing properties, negotiating deals, and advising homeowners on strategies to increase the value of their homes. Providing them with accurate and data-backed recommendations can enable them to better serve their clients and achieve successful sales.

## Data Understanding
The dataset I will use is the King County House Sales dataset, which contains information about house sales in a northwestern county. The dataset is provided in the kc_house_data.csv file in the data folder of the project's GitHub repository.
The data utilized in this project is kc_house_data.csv file as it provides relevant information for the analysis process. These columns below provide essential information about the houses in the dataset, which can be used for various analyses, such as predicting house prices, understanding the relationship between different features, or exploring the housing market trends.

### Column Names and Descriptions for King County Data Set
* `id` - Unique identifier for a house
* `date` - Date house was sold
* `price` - Sale price (prediction target)
* `bedrooms` - Number of bedrooms
* `bathrooms` - Number of bathrooms
* `sqft_living` - Square footage of living space in the home
* `sqft_lot` - Square footage of the lot
* `floors` - Number of floors (levels) in house
* `waterfront` - Whether the house is on a waterfront
  * Includes Duwamish, Elliott Bay, Puget Sound, Lake Union, Ship Canal, Lake Washington, Lake Sammamish, other lake, and river/slough waterfronts
* `view` - Quality of view from house
  * Includes views of Mt. Rainier, Olympics, Cascades, Territorial, Seattle Skyline, Puget Sound, Lake Washington, Lake Sammamish, small lake / river / creek, and other
* `condition` - How good the overall condition of the house is. Related to maintenance of house.
  * See the [King County Assessor Website](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r) for further explanation of each condition code
* `grade` - Overall grade of the house. Related to the construction and design of the house.
  * See the [King County Assessor Website](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r) for further explanation of each building grade code
* `sqft_above` - Square footage of house apart from basement
* `sqft_basement` - Square footage of the basement
* `yr_built` - Year when house was built
* `yr_renovated` - Year when house was renovated
* `zipcode` - ZIP Code used by the United States Postal Service
* `lat` - Latitude coordinate
* `long` - Longitude coordinate
* `sqft_living15` - The square footage of interior housing living space for the nearest 15 neighbors
* `sqft_lot15` - The square footage of the land lots of the nearest 15 neighbors

## Modeling
We used the following regression models:

* Simple Linear Regression model - Price vs Sqft_living
* Multiple Linear Regression model - Price vs sqft_living + sqft_living15 + sqft_above
* Multiple Linear Regression model - Price vs sqft_living + sqft_living15 + sqft_above + bedrooms 
* Multiple Linear Regression model - Price vs sqft_living + sqft_living15 + sqft_above + bedrooms + bathrooms
* Multiple Linear Regression model - Price vs sqft_living + sqft_living15 + sqft_above + bedrooms + bathrooms + grade

## Conclusion

Univariate Analysis

* In the year 2014 more houses were sold as compared to hoses sold in 2015.


* Most Houses in King County  were sold on the 4th and 5th  month of the year.


* Most houses in King County had 3 bedrooms followed by 4 bedrooms per house.


* Most of the houses had 2.5 bathrooms. Houses with more bathrooms and bedrooms had the highest prices.


* Most of the houses had no waterfront and no view however, the houses with a waterfront and a view had the highest prices.


* Most houses were in average condition and the houses with very good condition had the highest prices.



## Regression Model
* The multiple linear regression model is better than the two simple regression models as it had a higher R-squared value. This shows that categorical variables had a positive effect on the prices as illustrated in the univariate analysis.

* Therefore adding these variables to the predictive model made the model to be a bit stronger.

* In conclusion the real estate agency should review the sqft_living, sqft_living15, sqft_above, bedrooms, bathrooms, and grade when setting their house prices as there is a linear relationship between these variables.

* Factors like bathrooms, bedrooms, having a waterfront, and an excellent view have a positive effect on house prices. Lastly, the house prices seemed to have increased in 2015 they should therefore consider inflation when setting house prices in the future.


## Non-Technical Presentation

To access the non-technical presentation click here [Link](https://docs.google.com/presentation/d/1TOd9Cb0dX8W5OLbUASLv89wSEjf93IByFdxn-rfN59U/edit?usp=sharing)
