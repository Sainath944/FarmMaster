## CropFusionAI Backend  

This repository powers the CropFusionAI Frontend [here](https://github.com/deepeshdm/CropFusionAI), providing:  
- Model training data & notebooks  
- Trained ML models for crop & fertilizer classification  
- FastAPI backend exposing models via REST APIs  

🔗 **API Docs**: [Click here](https://8080-797137136eb6451193a1f8c64a951490.patr.cloud/docs)  

### 🚀 API Usage  

#### Crop Recommendation API  
```python
import requests
url = "https://8080-797137136eb6451193a1f8c64a951490.patr.cloud/crop_recommend"
payload = {"array": [55,44,33,40,75,6.5,300]}
response = requests.post(url, json=payload)
print(response.json())
