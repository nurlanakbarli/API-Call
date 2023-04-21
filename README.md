
**Dimension Group API**

This Python script provides functionality to interact with the Dimension Group API of a certain module (in this case, modul_name). It allows you to create, modify, and delete dimension groups by sending HTTP requests to a certain URL using the requests library.

**Prerequisites**

Before running this script, make sure you have the following installed:

- Python 3
- requests library


**Usage**

Clone or download this repository to your local machine.
Open the script (APIcalls_fonction.ipynb) in your Python editor of choice.
Modify the following variables to match your environment:


Save the modifications and run the script. It will perform the following actions:

_Login to the API using the provided credentials
Load the dimension group data from the JSON files
Create each dimension group by sending POST requests to the API
Modify each dimension group by sending PUT requests to the API
Delete a dimension group by sending a DELETE request to the API


**Definition**

This code defines a function called "call_api" that takes several arguments, including the HTTP method to use ("method"), a URL to make the API call to ("url"), an authorization token ("token"), and various other parameters related to the data being sent in the request. Depending on the value of "method", the function sends a POST, PUT, or DELETE request to the specified URL using the provided data, and returns the response from the server.

The code then has a loop that iterates over each element in the "dim_group_list" list. For each element, it constructs API endpoint URLs by concatenating the base "APIcall" string with the current "dim_group_name_list" and "dim_group_name_listPut" elements at the current index. It then runs another loop that iterates over the methods 'POST', 'PUT', and 'DELETE', and calls the "call_api" function with the appropriate arguments for each method. After each API call, the code waits for 5 seconds using "time.sleep()", prints the HTTP status code of the response, and displays the response text.

Overall, this code seems to be making API calls to create, update, or delete dimension groups using the specified endpoint URLs and data. The specific behavior depends on the values in the "dim_group_list" and "dim_group_listPut" lists, as well as the other parameters passed to the "call_api" function.
