
---

## 📄 `payment.md`

```md
# Payment

Stores Razorpay payment transaction details.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| orderId | String | Yes | – | Internal order reference ID. |
| productId | ObjectId | No | – | Linked product. |
| testId | ObjectId | No | – | Paid test. |
| razorpayOrderId | String | No | – | Razorpay order ID. |
| razorpayPaymentId | String | No | – | Razorpay payment ID. |
| razorpaySignature | String | No | – | Razorpay signature. |
| amount | Number | Yes | – | Paid amount. |
| status | String | No | CREATED | Payment status. |

---

## Indexes

- Index: `orderId`

---

## Example Document

```json
{
  "orderId": "ORD-20260117-001",
  "productId": "65f1a2c9e1234567890aaaa",
  "testId": "65f1a2c9e1234567890bbbb",
  "razorpayOrderId": "order_Mn12Ab",
  "razorpayPaymentId": "pay_Mn34Cd",
  "amount": 20,
  "status": "SUCCESS"
}
