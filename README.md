
# 🤖 FreeGPT 3.5 API Service 🚀

![FreeGPT 3.5 Logo](https://aizhinan.cc/wp-content/uploads/2023/04/FreeGPT.one%E5%AE%98%E7%BD%91%E5%85%A5%E5%8F%A3-aizhinan.cc.png)

## 📝 Description
This is a FreeGPT 3.5 API service that is available 24/7 without requiring an API key. The service has a rate limit of 1 request per second.

## 🚀 How to Use
### Base URL
https://freegpt35-y2kl.onrender.com/v1/Chat/completions

### Payload
```json
{
  "messages": "Messages Here Each Message Is separated By comma"
}
```

### 🚨 Example Curl Request
```bash
curl -X POST "https://freegpt35-y2kl.onrender.com/v1/Chat/completions" \
-H "Content-Type: application/json" \
-d '{"messages": "user:hi, Ai: hello, User: what is your Name?"}
```

### 📦 Example Response
```json
{
  "model": "freegpt-3.5",
  "choices": [
    {
      "message": {
        "role": "assistant",
        "content": "Hello! My name is FreeGPT-3.5. I am an AI model developed by FreeGpt_Api. How can I assist you today?"
      }
    }
  ]
}
```

### 🔄 System Prompt Example
```bash
curl -X POST "https://freegpt35-y2kl.onrender.com/v1/Chat/completions" \
-H "Content-Type: application/json" \
-d '{"messages": "system:The Value of A Is 10, User: what is Value Of a?"}'
```

### 📋 System Prompt Response
```json
{
  "model": "freegpt-3.5",
  "choices": [
    {
      "message": {
        "role": "assistant",
        "content": "The value of \\(a\\) is 10."
      }
    }
  ]
}
```

### ❌ Error Responses
- Authentication Error: 500
- External API Not Working: 500
- Internal Server Error: 500
- Rate Limit Error: 429 (1 request per second)

## 🙌 Support
If you find this service helpful, you can support me at [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/paytojaypaun)
