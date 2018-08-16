# TransferWise API Postman collection
A Postman collection containing example requests to demonstrate and test the [TransferWise public API](https://api.transferwise.com).

For use with the Postman client: [download it here](https://www.getpostman.com/).

# Use

Import the TW-API.postman_collection.json file to Postman to add all of the REST calls to your app in a dedicated collection.

Import the TW-API-ENVIRONMENT.postman_environment.json file to Postman to add the "Environment" used to manage variables for use in the calls.

# Setting up your Environment variables
Depending on your use case some features may or may not be available to you, this affects how you set up your environment.

## Personal Token users
Just set the `TOKEN` variable

## Banks and Businesses 
Set the `clientId`, `secret` and `clientRedirectUri` variables and use [this guide](https://api-docs.transferwise.com/v1/api-basics/authentication-and-headers#authentication-for-banks-and-businesses) to get a token for a user.

The OAuth token generation endpoints (`/oauth/token`) have tests that automatically set your `REFRESH` and `TOKEN` variables when you sucessfully generate them
