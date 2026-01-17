
---

## 📄 `linkedAccount.md`

```md
# LinkedAccount

Stores Razorpay linked account details for Cognito users.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| cognitoId | String | Yes | – | AWS Cognito User ID. |
| razorpayAccountId | String | No | – | Razorpay linked account ID. |
| onboardingStatus | String | No | pending | Razorpay onboarding status. |
| oauthAccessToken | String | No | – | OAuth access token. |
| oauthRefreshToken | String | No | – | OAuth refresh token. |
| connectedAt | Date | No | – | Account connection date. |
| lastValidatedAt | Date | No | – | Last validation timestamp. |
| status | String | No | active | Account status. |

---

## Indexes

- Index: `cognitoId`
- Index: `razorpayAccountId`

---

## Example Document

```json
{
  "cognitoId": "ap-south-1:merchant123",
  "razorpayAccountId": "acc_12345",
  "onboardingStatus": "linked",
  "status": "active"
}
