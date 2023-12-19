# Connection Details 

Python script used to find and check details about all connections, in both SafariJV and O'Reilly Private Cloud. 


## Use: 
Two files: 
- get_details.py: Main script that processes the request. 
- lookup_file.txt: Lookup file that is used when the Auth0 Connection ID is unknown. 

### usage: 

get_details.py [connection_id] or  [connection_name]  --cert (optional) --full (optional)

- If connection_id is know, it is usually best to use that. 
- Connection_name can be used, the script will check the lookup_file.txt to find the connection_id which is required by the Auth0 API. 
- --cert is an optional parameter, if used, it will return the full certificate in the results. 
- --full is also optional. If this is used, the results will include a full dump of the JSON results from the API call. 

## Installation/Requirements 

### Requires these packages:  
argparse
requests
json
os
dotenv 

### You will also need a .env file:

- Should have client_id and client_secret for the SafariJV Public tenant. 
- Please feel free to reach out to others on the O'Reilly Platform Integration team to get an already configured .env file to get started.  

## Note: 

- This tool may be superceeded by the Django Admin app that is forthcoming.  


Dec 18, 2023

