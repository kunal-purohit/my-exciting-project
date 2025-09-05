# Git Assignment Part II  

## 1. README for `country-capital-api`  

### Project Overview  
The **Country-Capital API** is a Python + Flask based microservice that returns the **country name** when provided with a **capital city**.  
It is lightweight, fast, and served using **Uvicorn (ASGI server)**.  

An organizational microservice endpoint is available at:  

```
https://example.com/country-capital/<query-params>
```  

This endpoint can be consumed by other projects across the organization.  

---

### Setup Instructions (Local Development)  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/<org>/country-capital-api.git
   cd country-capital-api
   ```  

2. **Create and Activate Virtual Environment**  
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac  
   venv\Scripts\activate      # Windows
   ```  

3. **Install Dependencies**  
   ```bash
   pip install -r requirements.txt
   ```  

4. **Run the Application**  
   ```bash
   uvicorn main:app --reload
   ```  

   The API will be available at:  
   ```
   http://127.0.0.1:8000
   ```  

---

### Prerequisites  

- Python 3.8+  
- pip (Python package manager)  
- Virtual environment (recommended)  
- Uvicorn & Flask installed  

---

## 2. .gitignore File  

```gitignore
# Ignore build directory
/build/

# Ignore environment variable files
*.env

# Ignore test logs
/test-runs/logs/

# Ignore all CSV files
*.csv
```  

---

## 3. Pull Request (PR) Description  

**PR Title:**  
```
feat/FEAPP-420: Allow customer notification via WhatsApp
```  

**PR Description:**  

**WHAT:**  
Introduced a new feature that allows customers to specify their WhatsApp number as an additional channel for product update notifications. If a customer provides a WhatsApp number, notifications will now be sent to both their email and WhatsApp.  

**WHY:**  
A significant portion of customers requested the ability to receive notifications via WhatsApp, considering it a more immediate and convenient communication channel compared to email. This feature addresses that feedback and enhances customer engagement.  

**Notes:**  
- Updated notification service to support multiple channels.  
- Developers setting up local environments should ensure they have valid WhatsApp API credentials in their `.env` file.  

**PR Reviewers:**  
- Add all teammates including the team lead for review.  

---

**End of Assignment Part II**  
