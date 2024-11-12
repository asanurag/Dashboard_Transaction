# Transaction-Dashboard

# MERN Stack Coding Challenge Solution

## Backend Task

### Data Source

- **THIRD PARTY API URL:** `https://s3.amazonaws.com/roxiler.com/product_transaction.json`
- **REQUEST METHOD:** `GET`
- **RESPONSE FORMAT:** `JSON`

2. **APIs:**
   - **List Transactions:**
     - API supports search and pagination on product transactions.
     - Matching the search text on product title/description/price and return matching product transactions.
     - Default pagination values: `page = 1`, `per page = 10`.
   - **Statistics:**
     - Total sale amount of the selected month.
     - Total number of sold items of the selected month.
     - Total number of not-sold items of the selected month.
   - **Bar Chart:**
     - Price range and the number of items in that range for the selected month.
     - Ranges:
       - 0 - 100
       - 101 - 200
       - 201 - 300
       - 301 - 400
       - 401 - 500
       - 501 - 600
       - 601 - 700
       - 701 - 800
       - 801 - 900
       - 901 - above
   - **Pie Chart:**
     - Unique categories and number of items from that category for the selected month.
     - Example:
       - X category: 20 items
       - Y category: 5 items
       - Z category: 3 items
   - **Combined Response:**
     - Fetched data from all the above APIs, combined the response, and sent a final combined JSON response.

## Frontend Task

- Using the APIs to build the following on a single page:
  - **Transactions Table:**
    - List transactions using the API.
    The month dropdown should display options from January to December.
    The default selected month is March.
    - Table lists transactions of the selected month using the API.
    - Searching transactions box matches title/description/price and filters the transactions of the selected month using the API.
    - Clearing the search box displays the initial list of transactions for the selected month using the API.
    - Pagination uses API to control load data for the next/previous page.
  - **Transactions Statistics:**
    - Using the API, display the total sale amount, total sold items, and total not sold items for the selected month from the dropdown.
  - **Transactions Bar Chart:**
    Using the API, Display the price range and the number of items in that range for the selected month.
  - Using Tailwind CSS for styling.

## Database

- Using MongoDB Atlas for the database.

### Note

Feel free to implement your design to change the look and feel.
