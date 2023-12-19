# Offboarding tools 

Python script used to find unused/under used Auth0 connections.  Current version only checks the 


## Use: 

There are four scripts: 

- get_details.py : Used to gather all current connections in the SafariJV tenant. 
- check_logs.py: Uses the list created by get_details.py and find connections where thare are less than 4 entries
- remove_apps.py: removes all applications on the connection ID that is provided. 
- delete_connections.py:  creates a back up of the connection and then deletes it. 

### Requires these packages: 

- requests
- json 
- datetime 
- pandas
- os 
- dotenv 
- argparse 

### You will also need a .env file:
- Should have client_id and client_secret for the SafariJV Public tenant. 

- Please feel free to reach out to others on the O'Reilly Platform Integration team to get an already configured .env file to get started.  

### Note: 

This will be updated in 2024 to work from the perspective of the accounts that are expiring rather than from the connection with little or no usage.   

The updated script will run everyday from a Jenkins job.  




