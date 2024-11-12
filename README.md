# Transaction-Dashboard

# MERN Stack Coding Challenge

## Backend Task

### Data Source

- **THIRD PARTY API URL:** `https://s3.amazonaws.com/roxiler.com/product_transaction.json`
- **REQUEST METHOD:** `GET`
- **RESPONSE FORMAT:** `JSON`

2. **APIs:**
   - **List Transactions:**
     - API are supporting search and pagination on product transactions.
     - Match search text on product title/description/price and return matching product transactions.
     - Default pagination values: `page = 1`, `per page = 10`.
   - **Statistics:**
     - Total sale amount of the selected month.
     - Total number of sold items of the selected month.
     - Total number of not sold items of the selected month.
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
     - Fetched data from all the above APIs, combine the response, and send a final combined JSON response.

## Frontend Task

- Using the APIs to build the following on a single page:
  - **Transactions Table:**
    - List transactions using the API.
    - Month dropdown should display options from January to December.
    - Default selected month is March.
    - Table lists transactions of the selected month using the API.
    - Search transactions box matches title/description/price and filters the transactions of the selected month using the API.
    - Clearing the search box displays the initial list of transactions for the selected month using the API.
    - Pagination controls load data for the next/previous page using the API.
  - **Transactions Statistics:**
    - Display total sale amount, total sold items, and total not sold items for the selected month from the dropdown using the API.
  - **Transactions Bar Chart:**
    - Display the price range and the number of items in that range for the selected month using the API.

## Database

- Using MongoDB Atlas for your database.

### Note

Feel free to implement your own design to change the look and feel.
