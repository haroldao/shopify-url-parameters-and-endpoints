# Shopify URL parameters and endpoints

When working with Shopify URLs, you can use various query parameters and JSON endpoints to control the page behavior and interact with Shopify's storefront data. Below are some commonly used parameters and a list of useful JSON endpoints.

### Common Shopify URL Parameters

- `?_fd=0`: Prevents domain forwarding, ensuring the URL remains unchanged when navigating between Shopify and your custom domain.
- `?pb=0`: Hides the Shopify preview bar, providing a cleaner view of the page, useful for screenshots or sharing the page without the preview tools visible.
- `?view=<view-name>`: Allows you to load a specific alternate template view for a page, useful for testing or displaying custom views (e.g., ?view=wholesale).
- `?sort_by=<filter>`: Applies a filter for the collection page, allowing users to sort or display items based on certain parameters (e.g., ?sort_by=price-ascending).
- `?customer_posted=<true|false>`: Used after submitting forms related to customer data (e.g., after submitting a contact form)
- `?q=<search-query>`: Performs a search on the store based on the query entered (e.g., ?q=shoes).
- `?ab=<?>`: Used for ?
- `?sc=<?>`: Used for ?
- `?variant=<variant-id>`: Automatically selects a specific variant on the product page when loading (e.g., ?variant=123456789).
- `?checkout[shipping_address][country]=<country>`: Prefills checkout fields, in this case, the shipping country.
- `?preview_theme_id=<theme-id>`: Allows you to preview a specific theme on your store without publishing it.
- `?page=<page-number>`: Used for pagination on collection pages, allowing users to navigate between multiple pages of products.
- `?type=<collection-type>`: Collection type query to filter products by specific types.
- `?filter=<filter-query>`: Applies filtering options to collections, such as price or tag filters.


### Shopify JSON Endpoints:

- `/cart/counts.json`: Retrieves the current number of items in the cart in JSON format.
- `/cart.js`: Retrieves the full cart contents in JSON format, including items, quantities, and total price.
- `/products/<product-handle>.js`: Retrieves product details in JSON format, including variants, price, and availability.
- `/collections/<collection-handle>/products.json`: Retrieves a list of products within a specific collection.
- `/search/suggest.json?q=<query>&resources[type]=product`: Provides product search suggestions in JSON format based on the query.
- `/pages/<page-handle>.json`: Retrieves details for a specific page in JSON format.
- `/challenge`: Redirects to a challenge page, which Shopify uses for security purposes, like verifying the user is human when suspicious behavior is detected.

<br>

**If you have any suggestions or improvements for this repository, feel free to open a pull request on GitHub!**
