```markdown
# Aigeon AI Google Hotels API

## Overview

The Aigeon AI Google Hotels API is a powerful server application designed to facilitate seamless integration with Google Hotels search capabilities. This server leverages the SerpAPI to provide comprehensive hotel search functionalities, allowing users to query for hotel information based on a wide array of parameters. The application is built using Python and utilizes the FastMCP server framework for efficient and scalable operations.

## Features Overview

- **Comprehensive Search Parameters**: The API allows users to perform detailed hotel searches using a variety of parameters such as location, check-in/out dates, number of guests, price range, property types, amenities, and more.
- **Customization Options**: Users can customize their search queries with options like language, currency, sorting preferences, and filtering by hotel class or brand.
- **Support for Vacation Rentals**: In addition to hotels, the API supports searches for vacation rentals, with specific parameters for bedrooms and bathrooms.
- **Advanced Filtering**: The API provides advanced filtering options such as free cancellation, special offers, eco-certification, and more.
- **Pagination and Caching**: The API supports pagination through next page tokens and offers caching options to optimize search performance.

## Main Features and Functionality

1. **Search Hotels**: The core functionality of the API is to perform hotel searches based on user-defined parameters. It utilizes the SerpAPI to fetch results from Google Hotels, ensuring accurate and up-to-date information.

2. **Parameter Customization**: Users can define a wide range of parameters to tailor their search queries. This includes specifying the search query, check-in and check-out dates, geographical location, language, currency, and more.

3. **Filtering and Sorting**: The API allows users to filter results based on criteria such as price range, property type, amenities, rating, and brand. Additionally, results can be sorted by relevance, price, rating, or number of reviews.

4. **Support for Vacation Rentals**: The API extends its functionality to include vacation rental searches, with parameters for specifying the number of bedrooms and bathrooms.

5. **Advanced Options**: Users can enable advanced options such as no-cache searches, asynchronous search submissions, and enterprise-level features like ZeroTrace mode.

## Main Functions Description

### `search_hotels`

The `search_hotels` function is the primary tool for querying hotel information. It accepts a comprehensive set of parameters that allow users to customize their search queries extensively. Below is a description of the key parameters:

- **q**: The search query string used in a typical Google Hotels search.
- **check_in_date / check_out_date**: Dates for check-in and check-out in the format YYYY-MM-DD.
- **gl / hl**: Country and language codes for localizing the search results.
- **currency**: Specifies the currency for price display.
- **adults / children / children_ages**: Defines the number of adults and children, along with their ages.
- **sort_by**: Determines the sorting order of the results (e.g., by price, rating, or reviews).
- **min_price / max_price**: Sets the price range for the search results.
- **property_types / amenities**: Filters results by property type and available amenities.
- **rating / brands / hotel_class**: Filters results by rating, brand, and hotel class.
- **free_cancellation / special_offers / eco_certified**: Filters for specific features like free cancellation, special offers, and eco-certification.
- **vacation_rentals / bedrooms / bathrooms**: Parameters specific to vacation rental searches.
- **next_page_token / property_token**: Used for pagination and retrieving detailed property information.
- **no_cache / aasync / zero_trace**: Advanced options for caching, asynchronous operations, and enterprise-level privacy.

This function is designed to provide users with a flexible and powerful tool for accessing hotel data, making it suitable for a wide range of applications in travel and hospitality industries.
```
