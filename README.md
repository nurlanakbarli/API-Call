# API-Call

Hello world !

first we import necessary libraries such as json, requests and urllib. After that it is necessary to determine the url address, the username, the password and the name of the module.

The requests.get(url+'/ping') line sends a GET request to the URL url+'/ping'. r.json() converts the server's response from JSON format to a Python dictionary. The requests.post(url+'/login', json={"identifier":user,"password":password}) line sends a POST request to the URL url+'/login' with a JSON payload containing the user's identifier and password. r.json()['token'] extracts the token from the JSON response that is returned by the server.

After that we have 2 lines. The first line sets the path variable to the file path where the JSON file is located.The second line uses the json.load() method to read the contents of the JSON file. 


The three lines of code extract the "name" key value from each dictionary element in json_data and appends it to dim_group_name_list, and also convert each element in json_data to a JSON formatted string representation and append it to dim_group_list.


After we define the precise address of the APIcall


We have also "for" loop. This for loop appears to generate a list of API calls for each dimension group in dim_group_list by appending the name of the dimension group to a base API URL or endpoint.


