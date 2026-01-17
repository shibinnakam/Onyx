
---

## 📄 `Product.md`

```md
# Product Schema

Represents a hardware device (sensor / weight machine).

## Fields

- `productId` (String, unique)  
  Physical device ID (QR / Scanner)

- `productName` (String)  
  Name of the device

- `installedLocation.address` (String)  
  Installed address

- `installedLocation.placeType` (String)  
  Railway station, school, hospital, etc.

- `cognitoId` (String)  
  Owner Cognito ID

- `status` (Enum)  
  ACTIVE | INACTIVE | MAINTENANCE

