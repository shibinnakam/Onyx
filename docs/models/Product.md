
---

## 📄 `product.md`

```md
# Product

Represents a physical hardware device (sensor / machine).

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| productId | String | Yes | – | Unique device identifier (QR / scanner). |
| productName | String | Yes | – | Name of the hardware device. |
| installedLocation.address | String | No | – | Installation address. |
| installedLocation.placeType | String | No | – | Location type (railway station, school, etc.). |
| cognitoId | String | Yes | – | Cognito ID of the device owner. |
| status | String | No | ACTIVE | Current device status. |

---

## Indexes

- Unique: `productId`

---

## Example Document

```json
{
  "productId": "WM-10023",
  "productName": "Smart Weight Machine",
  "installedLocation": {
    "address": "Ernakulam Railway Station",
    "placeType": "railway_station"
  },
  "cognitoId": "ap-south-1:merchant123",
  "status": "ACTIVE"
}
