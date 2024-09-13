Project Overview

The dataset contains information on various restaurants, including attributes such as name, online ordering availability, table booking options, ratings, popular dishes, and approximate costs. The cleaning process was aimed at removing unnecessary information and ensuring that the data was consistent and ready for analysis.

1. Initial Dataset Overview

The raw dataset contained multiple columns related to restaurant details, including contact information, reviews, and metadata. The key issues addressed in the raw data included:

Redundant columns that were not necessary for analysis.

Missing values in some fields.

Data formatting inconsistencies, particularly in ratings and cost columns.

2. Data Cleaning Steps Applied

2.1. Column Removal

Several columns from the raw data were removed to streamline the dataset:

URL, address, phone, reviews_list, menu_item, votes, cuisines, rest_type: These columns were removed as they were either redundant or not directly relevant to the desired analysis of restaurant attributes.

2.2. Handling Missing Data

NaN values: Missing values were addressed to ensure a complete and usable dataset. This step involved either filling or removing null entries where applicable, particularly in categorical columns like Dish_liked.

2.3. Data Type Standardization

Rate: The ratings, stored as strings in the format "4.1/5", were kept as is, possibly for further parsing or direct use.

Approx_cost(for two people): The approximate cost values, though stored as strings in the format with potential symbols or commas, were retained for ready interpretation.

2.4. Duplicate and Redundant Data

Duplicate records: Any duplicate rows in the dataset were removed to ensure that each entry corresponded to a unique restaurant.

3. Final Dataset Overview

After the cleaning process, the dataset contains 7 columns and 8,250 entries, including:

Name: Restaurant name.

Online_order: Indicates whether the restaurant offers online ordering (Yes/No).

Book_table: Indicates whether the restaurant offers table booking (Yes/No).

Rate: The restaurant's rating (e.g., "4.1/5").

Dish_liked: Dishes liked by the customers.

Approx_cost(for two people): Approximate cost for two people as provided.

Unnamed: 0: A leftover index column, which may serve as an index for internal data tracking.

4. Conclusion

The cleaning process was successfully completed, reducing the dataset to its essential components while ensuring data quality and consistency. The resulting dataset is now optimized for analysis, focusing on key restaurant attributes such as ratings, popular dishes, and costs.
