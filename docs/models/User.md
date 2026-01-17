# User Schema

This schema stores user information authenticated via AWS Cognito.

## Fields

- `cognitoId` (String, unique, indexed)  
  AWS Cognito User ID

- `name` (String)  
  User full name

- `phone` (String, unique)  
  User phone number

- `email` (String, unique)  
  User email address

- `location.address` (String)  
  User address

- `isPhoneVerified` (Boolean, default: true)  
  Phone verification status


