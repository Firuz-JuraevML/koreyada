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

### 1. Login & Sign up Endpoints 
<details>
<summary> 📌 POST /login/ </summary>

### Login Endpoint 
* User login page 

> Request body: 
```json
{
  "login": "fjuraev",
  "password": "Ewing0605"
}
```

> Response (200): 
```json
{
 "user_id": 233
 "user_name": "Firuz Juraev"
}
```
</details>




<details>
<summary> 📌 POST /sign_up/ </summary> 
  
### Sign up Endpoint   
* User sign up
  
> Request body: 
```json
{
  ""
  "login": "fjuraev",
  "password": "Ewing0605"
}
```

> Response (200): 
```json
{
 "message": "Successfully registered" 
}
```
</details>


<details>
<summary> 📌 POST /forget_password/ </summary> 

### Forget Password Endpoint  
* User forgot password

> Request body: 
```json
{
  ""
  "email": "example@gmail.com",
}
```

> Response (200): 
```json
{
 "message": "Email found & and sent" 
}
```
</details>

--- 


### 2. Main Page API Endpoints

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
<summary> 📌 GET /main_categories/ </summary>

### Categories Endpoint 
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


<details>
<summary> 📌 GET /latest_news/ </summary>

### Latest News Endpoint 
* Returns the latest posted news 

> Response (200): 
```json
{
  "1": {  "news_id": 23
          "news_title_en": "The rules for getting E-7 have changed",
          "news_title_uz": "E-7 olish qoidalari o'zgardi",
       }
}
```
</details>


<details>
<summary> 📌 GET /latest_articles/ </summary>

### Latest Articles Endpoint 
* Returns the latest posted articles 

> Response (200): 
```json
{
  "1": {  "article_id": 24
          "article_title_en": "How to open a bank account in Korea",
          "article_title_uz": "Qanday qilib bank hisob raqam ochish", 
       }
}
```
</details>


<details>
<summary> 📌 GET /featured_businesses/ </summary>

### Latest Articles Endpoint 
* Returns the latest posted articles 

> Response (200): 
```json
{
  "1": {  "article_id": 24
          "article_title_en": "How to open a bank account in Korea",
          "article_title_uz": "Qanday qilib bank hisob raqam ochish", 
       }
}
```
</details>

--- 


### 3. Categories Page Endpoints 
<details>
<summary> 📌 POST /category_businesses/ </summary>

### Category Businesses Endpoint 
* Returns the list of registered businesses

> Request body: 
```json
{
  "category_id": 1 
}
```

> Response (200): 
```json
{
  "1": {  "business_id": 12
          "article_title_en": "How to open a bank account in Korea",
          "article_title_uz": "Qanday qilib bank hisob raqam ochish", 
       }
}
```
</details>



<details>
<summary> 📌 POST /category_articles/ </summary> 
  
### Category Articles Endpoint 
* Returns the list of articles related to the selected category 

> Request body: 
```json
{
  "category_id": 1 
}
```

> Response (200): 
```json
{
  "1": {  "business_id": 12
          "article_title_en": "How to open a bank account in Korea",
          "article_title_uz": "Qanday qilib bank hisob raqam ochish", 
       }
}
```
</details>


<details>
<summary> 📌 POST /category_news/ </summary> 
  
### Category News Endpoint 
* Returns the list of news related to the selected category 

> Request body: 
```json
{
  "category_id": 1 
}
```

> Response (200): 
```json
{
  "1": {  "business_id": 12
          "article_title_en": "How to open a bank account in Korea",
          "article_title_uz": "Qanday qilib bank hisob raqam ochish", 
       }
}
```
</details>

--- 







