
---

## 📄 `Order.md`

```md
# Order Schema

Created after successful payment.

## Fields

- `orderId` (String, unique)  
  Order reference ID

- `productId` (ObjectId)  
  Device used

- `testId` (ObjectId)  
  Test performed

- `paymentId` (ObjectId)  
  Payment reference

- `orderStatus` (Enum)  
  PLACED | COMPLETED | CANCELLED

