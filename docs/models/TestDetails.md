
---

## 📄 `testDetails.md`

```md
# TestDetails

Defines tests available on the device with pricing.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| testName | String | Yes | – | Name of the test. |
| description | String | No | – | Description of the test. |
| amount | Number | Yes | – | Cost of the test. |
| unit | String | Yes | – | Measurement unit (weight, height, bp). |

---

## Indexes

- None

---

## Example Document

```json
{
  "testName": "Weight Check",
  "description": "Measures body weight",
  "amount": 20,
  "unit": "weight"
}
