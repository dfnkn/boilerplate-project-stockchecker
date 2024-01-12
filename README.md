# Stock Price Checker

This is the boilerplate for the Stock Price Checker project. Instructions for building your project can be found at https://freecodecamp.org/learn/information-security/information-security-projects/stock-price-checker

# Requirements

    - [ ] You can provide your own project, not the example URL.

    - [ ] You should set the content security policies to only allow loading of scripts and CSS from your server.

    - [ ] You can send a GET request to /api/stock-prices, passing a NASDAQ stock symbol to a stock query parameter. The returned object will contain a property named stockData.

    - [ ] The stockData property includes the stock symbol as a string, the price as a number, and likes as a number.

    - [ ] You can also pass along a like field as true (boolean) to have your like added to the stock(s). Only 1 like per IP should be accepted.

    - [ ] If you pass along 2 stocks, the returned value will be an array with information about both stocks. Instead of likes, it will display rel_likes (the difference between the likes on both stocks) for both stockData objects.

    - [ ] All 5 functional tests are complete and passing.

    - [ ] Due to the requirement that only 1 like per IP should be accepted, you will have to save IP addresses. 

    - [ ] It is important to remain compliant with data privacy laws such as the General Data Protection Regulation. 
        - One option is to get permission to save the user's data, 
        - Other option would be to anonymize it. 
    
    - [ ] For this challenge, remember to anonymize IP addresses before saving them to the database. Some options:
        - hash the data
        - truncate data
        - set part of the ip address to 0

# Tests

    Write the following tests in tests/2_functional-tests.js:

    - [ ] Viewing one stock: GET request to /api/stock-prices/
    - [ ] Viewing one stock and liking it: GET request to /api/stock-prices/
    - [ ] Viewing the same stock and liking it again: GET request to /api/stock-prices/
    - [ ] Viewing two stocks: GET request to /api/stock-prices/
    - [ ] Viewing two stocks and liking them: GET request to /api/stock-prices/

## Example of usage of endpoints

    /api/stock-prices?stock=GOOG
    /api/stock-prices?stock=GOOG&like=true
    /api/stock-prices?stock=GOOG&stock=MSFT
    /api/stock-prices?stock=GOOG&stock=MSFT&like=true


