# SahayX – System Design  

---

## 1️⃣ System Overview  

SahayX is an *AI-powered triage platform* that connects:
- Government service platforms (UMANG, DigiLocker)
- Private local service providers (plumbers, clinics, freelancers)

The system compares both and recommends the best option based on user eligibility and convenience.

---

## 2️⃣ High-Level Architecture  

User  
→ Mobile App (Flutter / React Native)  
→ Amazon Lex (Voice + NLP)  
→ Amazon Bedrock (AI Triage Engine)  
→ AWS Lambda (Business Logic)  
→ UMANG API + Private Provider APIs  
→ DynamoDB + S3  
→ User Interface  

---

## 3️⃣ AI Workflow  

### Step 1: User Input  
User speaks or types:
> “I need a doctor”

Amazon Lex converts speech → text and extracts intent.

---

### Step 2: Intent & Eligibility  
Amazon Bedrock receives:
- User request  
- User profile (age, income, location)  

It determines:
- Service type  
- Whether government schemes apply  

---

### Step 3: Data Fetching  
AWS Lambda fetches:
- Government services from UMANG  
- Private providers from ONDC / local databases  

---

### Step 4: Recommendation  
System labels:
- *Green* → Government (Free)  
- *Blue* → Private (Paid)  

And sends results to the app.

---

## 4️⃣ Data Storage  

| Data | Storage |
|------|---------|
| User Profiles | DynamoDB |
| Documents | S3 |
| Services | DynamoDB |
| Analytics | QuickSight |

---

## 5️⃣ Security  

- Cognito for authentication  
- IAM for permissions  
- S3 encryption for documents  

---

## 6️⃣ Scalability  

- Serverless (Lambda + DynamoDB)  
- ONDC integration  
- Works across urban & rural regions  

---

## 7️⃣ Future Scope  

- More Indian languages  
- ONDC auto-onboarding  
- AI fraud detection  
- Predictive service needs  

---