
---

## 📄 `Payment.md`

```md
# Payment Schema

Stores Razorpay payment details.

## Fields

- `orderId` (String)  
  Internal order reference

- `productId` (ObjectId)  
  Linked product

- `testId` (ObjectId)  
  Paid test

- `razorpayOrderId` (String)
- `razorpayPaymentId` (String)
- `razorpaySignature` (String)

- `amount` (Number)
- `status` (Enum)  
  CREATED | SUCCESS | FAILED
