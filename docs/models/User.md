# User

Stores application users authenticated via AWS Cognito.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| cognitoId | String | Yes | – | AWS Cognito User ID (unique identifier). |
| name | String | Yes | – | Full name of the user. |
| phone | String | Yes | – | User phone number (unique). |
| email | String | Yes | – | User email address (unique). |
| location.address | String | No | – | User address. |
| isPhoneVerified | Boolean | No | true | Phone verification status after OTP. |

---

## Indexes

- Unique: `cognitoId`
- Unique: `phone`
- Unique: `email`

---

## Example Document

```json
{
  "cognitoId": "ap-south-1:abc123",
  "name": "Rahul Kumar",
  "phone": "9876543210",
  "email": "rahul@example.com",
  "location": {
    "address": "Kochi, Kerala"
  },
  "isPhoneVerified": true
}
