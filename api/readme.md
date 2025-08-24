### 📖 API Documentation 

[![My Skills](https://skillicons.dev/icons?i=python,fastapi,docker)](https://skillicons.dev) 




<details>
<summary>⚡ Status Codes</summary> 

| Code | Meaning                  | Usage Example |
|------|--------------------------|---------------|
| 200  | **OK**                   | Successful GET, PUT, or POST request |
| 201  | **Created**              | Resource successfully created (e.g., after POST) |
| 202  | **Accepted**             | Request accepted for processing but not completed yet |
| 204  | **No Content**           | Request succeeded but no content to return (e.g., after DELETE) |
| 400  | **Bad Request**          | Invalid request payload or missing parameters |
| 401  | **Unauthorized**         | Missing or invalid authentication credentials |
| 403  | **Forbidden**            | Authenticated but not allowed to access the resource |
| 404  | **Not Found**            | Requested resource does not exist |
| 409  | **Conflict**             | Resource conflict (e.g., duplicate data) |
| 422  | **Unprocessable Entity** | Validation error in request data |
| 500  | **Internal Server Error**| Generic server-side error |
| 503  | **Service Unavailable**  | Server temporarily down or overloaded |
</details> 

### 1. Main Page API Endpoints

<details>
<summary>📌 GET /main_statistics/</summary>
  
### Main Statistics Endpoint 
* Returns general statistics about the website: number of registered users, number of categories, number of registered businesses, etc. 

> Response (200): 
```json
{
  "n_users": 1250,
  "n_categories": 6,
  "n_businesses": 60,
  "n_articles": 20,
  "n_news": 45
}
```
</details>


<details>
<summary> 📌 GET /categories/ </summary>

### Main Statistics Endpoint 
* Returns categories with some information: visa, restaurants, money transfers, etc. 

> Response (200): 
```json
{
  "1": {  "category_id": 1
          "category_name_en": "Visa",
          "category_name_uz": "Viza", 
          "category_description_en": "Visa applications, renewals, and immigration assistance",
       }
}
```
</details>
