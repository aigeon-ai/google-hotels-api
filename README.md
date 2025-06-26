# Aigeon AI Google Hotels API

## Project Description

The `aigeon-ai.google-hotels-api` is a Python-based server application designed to interact with Google Hotels through the SerpAPI. It provides a robust interface for searching hotel accommodations with various customizable parameters, allowing users to tailor their search results based on specific needs such as location, dates, price range, amenities, and more. This project leverages the FastMCP framework to facilitate efficient and scalable API interactions.

## Features Overview

- Seamless integration with Google Hotels via SerpAPI.
- Customizable search parameters to refine hotel search results.
- Support for both hotel and vacation rental searches.
- Advanced filtering options including price, rating, property type, and amenities.
- Multi-language and multi-currency support.
- Asynchronous search capabilities for improved performance.

## Main Features and Functionality

- **Hotel Search**: Perform detailed searches for hotels using a wide range of parameters such as check-in/out dates, location, number of guests, and more.
- **Vacation Rentals**: Option to search specifically for vacation rentals with additional parameters like number of bedrooms and bathrooms.
- **Sorting and Filtering**: Sort results by relevance, price, rating, and more. Filter results based on price range, property type, amenities, and other criteria.
- **Internationalization**: Specify language and currency preferences to cater to international users.
- **Caching and Asynchronous Requests**: Utilize caching to optimize repeated queries and asynchronous requests for non-blocking operations.

## API Endpoints or Main Functions Description

### `search_hotels`

This function is the core of the application, providing a comprehensive interface for querying Google Hotels. It accepts numerous parameters to customize the search:

- **q**: Search query string.
- **check_in_date**: Check-in date in `YYYY-MM-DD` format.
- **check_out_date**: Check-out date in `YYYY-MM-DD` format.
- **gl**: Country code for search localization.
- **hl**: Language code for search localization.
- **currency**: Currency code for pricing.
- **adults**: Number of adults.
- **children**: Number of children.
- **children_ages**: Ages of children.
- **sort_by**: Sorting criteria.
- **min_price**: Minimum price filter.
- **max_price**: Maximum price filter.
- **property_types**: Filter by property type.
- **amenities**: Filter by amenities.
- **rating**: Filter by rating.
- **brands**: Filter by hotel brands.
- **hotel_class**: Filter by hotel class.
- **free_cancellation**: Filter for free cancellation.
- **special_offers**: Filter for special offers.
- **eco_certified**: Filter for eco-certified properties.
- **vacation_rentals**: Toggle between hotels and vacation rentals.
- **bedrooms**: Minimum number of bedrooms (for vacation rentals).
- **bathrooms**: Minimum number of bathrooms (for vacation rentals).
- **next_page_token**: Token for paginated results.
- **property_token**: Token for detailed property information.
- **no_cache**: Toggle to bypass cache.
- **aasync**: Toggle for asynchronous request handling.
- **zero_trace**: Enterprise feature for enhanced privacy.

## Configuration Parameters Explanation

The application uses environment variables for configuration:

- **SERP_API_KEY**: API key for authenticating requests to SerpAPI. This should be set in a `.env` file or environment variable.

## Installation Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/aigeon-ai.google-hotels-api.git
   cd aigeon-ai.google-hotels-api
   ```

2. **Install Dependencies**:
   Ensure you have Python installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Environment Setup**:
   Create a `.env` file in the root directory and add your SerpAPI key:
   ```plaintext
   SERP_API_KEY=your_serp_api_key
   ```

## Usage Instructions

1. **Start the Server**:
   Run the server using the following command:
   ```bash
   python server.py
   ```

2. **Perform a Search**:
   Use the `search_hotels` function with the desired parameters to perform a hotel search. Refer to the function's parameter list for customization options.

## Requirements/Dependencies

- Python 3.7+
- `requests`: For making HTTP requests.
- `pydantic`: For data validation and settings management.
- `python-dotenv`: For loading environment variables from a `.env` file.
- `mcp.server` and `fastmcp`: For server management and API handling.

This README provides a comprehensive guide to understanding, installing, and using the `aigeon-ai.google-hotels-api` project. For further details, refer to the code comments and documentation within the project files.