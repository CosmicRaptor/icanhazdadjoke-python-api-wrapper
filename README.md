# icanhazdadjoke-python-api-wrapper
A simple API wrapper for https://icanhazdadjoke.com/api

# Installation
- `pip install requests`
- Import the [src/connection.py](src/connection.py) into your code.

# Usage
  - Run the `random` method to get a random joke.
  - Run the `search` method with a query passed to search for jokes. Optionally, you can pass the page, and limit.
  - Note: While creating an instance of the `DadJoke` class, please pass in the response type you expect. Currently the API supports HTML, plain text and JSON return types. The library supports plain text and JSON returns.
 
# Example
 ```python

from src.connection import DadJoke

obj = DadJoke(text)
print(obj.random())  # Random joke
print(obj.search("oven", limit=5)  # Gives you upto 5 search results for the term "oven"
```
