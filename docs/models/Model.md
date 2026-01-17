
---

## 📄 `model.md`

```md
# Model

Defines a hardware model and supported tests.

---

## Schema Fields

| Field | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| model_name | String | Yes | – | Model name of the device. |
| version | String | Yes | – | Version of the model. |
| tests | ObjectId[] | No | – | Linked TestDetails IDs. |

---

## Indexes

- None

---

## Example Document

```json
{
  "model_name": "WM-Pro",
  "version": "v1.0",
  "tests": [
    "65f1a2c9e1234567890abcd"
  ]
}
