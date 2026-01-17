
---

## 📄 `LinkedAccount.md`

```md
# LinkedAccount Schema

Stores Razorpay linked account details for Cognito users.

## Fields

- `cognitoId` (String)  
  AWS Cognito User ID

- `razorpayAccountId` (String)  
  Razorpay linked account ID

- `onboardingStatus` (Enum)  
  pending | linked | failed

- `oauthAccessToken` (String)
- `oauthRefreshToken` (String)

- `connectedAt` (Date)
- `lastValidatedAt` (Date)

- `status` (String)
