
---

## 📄 `order.md`

```md
# Order

Created after successful payment.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| orderId | String | Yes | – | Unique order identifier. |
| productId | ObjectId | Yes | – | Device used for the test. |
| testId | ObjectId | Yes | – | Test performed. |
| paymentId | ObjectId | Yes | – | Linked payment record. |
| orderStatus | String | No | PLACED | Current order status. |

---

## Indexes

- Unique: `orderId`

---

## Example Document

```json
{
  "orderId": "ORD-20260117-001",
  "productId": "65f1a2c9e1234567890aaaa",
  "testId": "65f1a2c9e1234567890bbbb",
  "paymentId": "65f1a2c9e1234567890cccc",
  "orderStatus": "COMPLETED"
}
