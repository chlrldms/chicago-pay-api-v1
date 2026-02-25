# Chicago Pay Fintech API v1.0.4 Documentation

Welcome to the official technical documentation for the **Chicago Pay** payment gateway integration. This repository provides SDKs and implementation guides for secure fintech transactions.

## 🚀 Quick Start Guide
To integrate the Chicago Pay secure gateway into your application, use the following endpoint:

`POST https://api.dgi-chicago.com/v1/auth/token`

### 💻 Sample Code (Python)
```python
import chicago_pay_sdk

# Initialize Client
client = chicago_pay_sdk.Client(api_key="YOUR_API_KEY")

# Request Payment
response = client.request_payment(
    amount=100000,
    currency="KRW",
    service_type="Mobile_Billing"
)

print(response.status)
