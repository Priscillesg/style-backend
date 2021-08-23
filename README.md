# Warning: DO NOT MERGE

## Changes
I made some simple changes to enable Django token authentication. 
This includes the following.

1. Modifying the django settings file to use token authentication
2. Installing and using the package `dj-rest-auth` (Add it to your requirements file)
3. And updating the routes to use the package.

## How to Login and Logout
1. `curl -X POST http://localhost:8000/auth/login/ -d username=nshipman -d password=Test123` Returns: `{"key":"bed4d236ec94854d3d9a91ca1b02a00e3d9af347"}%`
2. Visit the `/auth/login` endpoint to use the GUI variation.
3. To logout `curl -X POST http://127.0.0.1:8000/auth/logout/ -H "Authorization: Token bed4d236ec94854d3d9a91ca1b02a00e3d9af347"`


`