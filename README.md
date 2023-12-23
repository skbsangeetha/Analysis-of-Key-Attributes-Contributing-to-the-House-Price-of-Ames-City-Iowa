# Analysis-of-Key-Attributes-Contributing-to-the-House-Price-of-Ames-City-Iowa

# Data Source
https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
The dataset of our analysis is a machine-learning dataset sourced from Kaggle. This dataset is particularly interesting for analytics due to its rich and diverse set of features that offer a comprehensive view of the real estate market. It includes a wide range of property attributes such as size, condition, quality, and amenities, allowing for a multifaceted analysis of factors that influence home values. The inclusion of both numerical and categorical data, such as square footage, number of rooms, and quality ratings, provides opportunities for both quantitative and qualitative analyses.

# Objective
The purpose of this report is to identify the features that are the most impactful on house prices so that residential construction companies can leverage these findings when building new homes.

# Challenges
This dataset presents notable challenges for analysis due to its time-series nature and the significant impact of external factors on 'SalePrice'. Firstly, the value of properties is heavily influenced by overarching market trends over time, meaning that prices are subject to fluctuations in the broader real estate market, such as the 2008-2009 financial crisis. Secondly, the age and recentness of renovations play a disproportionately large role in determining sale prices, with newer houses and those recently remodelled naturally fetching higher prices. To mitigate these biases and accurately assess the intrinsic value of properties based on their features, it was essential to normalize the data. This normalization process allows for a more focused analysis of the specific attributes of the houses, such as size, quality, and amenities, independent of market-wide trends and the age or renovation status of the properties. The analysis also needs to take into account the sales volume; while larger house usually sells for more, the sales are usually far between. We want to strike a balance and identify features that positively impact the house price with reasonable sales volume.

# Analysis
After a preliminary analysis of the dataset, ten features were short-listed to be our target for analysis:

* 'LotFrontage' (Linear feet of street connected to the property): Generally, a larger frontage indicates more accessibility and potential curb appeal, which can positively influence 'SalePrice'. However, its impact may be more nuanced depending on the location and layout of the property.

* 'LotArea' (Lot size in square feet): Larger lot areas can lead to higher prices due to increased space, but the correlation varies significantly based on the property's geographic location and the typical lot size in the area.

* 'MSSubClass' (The building class): This feature classifies the type of dwelling involved in the sale. While it provides valuable context, its direct correlation with 'SalePrice' may not be as strong as other features. The style and utility implied by the subclass can influence buyer preferences.

* 'BsmtQual' (Basement quality): High-quality basements can substantially increase a property's value, especially if they provide additional livable space or special amenities.

* 'TotalBsmtSF' (Total basement square feet): One of the top contributors. A larger basement area, particularly if well-finished, significantly enhances a property’s appeal and functionality, leading to higher sale prices.

* 'GrLivArea' (Above grade living area square feet): Another top contributor. This feature directly correlates with the property's size and usable space, making it a primary determinant of 'SalePrice'.

* 'FullBath' (Number of full bathrooms): Also among the top contributors. More bathrooms add convenience and luxury, thus increasing the property value.

* 'TotRmsAbvGrd' (Total rooms above grade, excluding bathrooms): This feature strongly influences 'SalePrice' as it reflects the overall space and utility of the property. More rooms typically equate to more space, which is desirable to buyers.

* 'GarageType' (Garage location and type): While it provides insight into the property's amenities, its impact on 'SalePrice' may be less direct compared to the garage's size or capacity.

* 'GarageCars' (Size of garage in car capacity): A significant contributor to 'SalePrice'. Properties with larger garages, typically accommodating more vehicles, tend to have higher sale prices due to the added convenience and storage space.

# Conclusions
Among these features, 'GrLivArea', 'TotalBsmtSF', 'FullBath', 'TotRmsAbvGrd', and 'GarageCars' stand out as the top five contributors to a high 'SalePrice'. These features collectively represent the property's size, functionality, and essential amenities, which are key determinants of value in the real estate market. Properties excelling in these aspects are likely to command higher prices, reflecting their desirability and utility to potential buyers. Based on these insights, a property with a larger 'GrLivArea' and 'TotalBsmtSF', at least 2 'FullBath', around 6-7 'TotRmsAbvGrd', and a 2-car 'GarageCars' capacity is likely to command the highest 'SalePrice' among the combinations of these attributes, while also being attractive to a broad segment of buyers. This combination balances spaciousness, utility, and market desirability, making it a potentially high-value configuration in the real estate market.
