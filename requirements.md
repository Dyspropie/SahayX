# SahayX – Requirements Specification  

## 1. Purpose  
This document defines the functional and non-functional requirements for *SahayX*, an AI-powered platform that connects users with both government and private services while prioritizing free and eligible government schemes.

The goal is to ensure that users never pay for a service they can legally receive for free.

---

## 2. Target Users  
- Rural and semi-urban citizens  
- Senior citizens  
- Low-income groups  
- Digitally inexperienced users  
- Local service seekers (healthcare, utilities, documents, etc.)

---

## 3. Core Functional Requirements  

### 3.1 User Authentication  
- Users must be able to sign up and log in using mobile number  
- Aadhaar-linked identity verification must be supported  
- User profile must store age, income range, and location  

---

### 3.2 Voice-Based Service Request  
- Users must be able to speak their service need  
- System must support Hindi, Tamil, and English  
- Speech must be converted into structured service requests  

---

### 3.3 AI Intent Recognition  
- The system must understand what service the user is requesting  
- It must classify the request (healthcare, utilities, documents, etc.)  

---

### 3.4 Eligibility Detection  
- The system must evaluate whether the user is eligible for any government schemes  
- It must warn users when a free government alternative exists  

---

### 3.5 Service Matching  
The platform must display:
- Government services (free/subsidized)  
- Private providers (paid)  
- Distance-based options within 5 km  

---

### 3.6 Comparison Interface  
- Government and private services must be shown side-by-side  
- Free services must be highlighted in green  
- Paid services must be highlighted in blue  

---

### 3.7 Service Booking / Redirection  
- Users must be able to book private services  
- Users must be able to open government portals (UMANG, DigiLocker, etc.)  

---

### 3.8 Document Handling  
- Users must be able to upload or link Aadhaar and other documents  
- Documents must be stored securely  

---

### 3.9 Notifications  
- Users must receive reminders for appointments  
- Users must receive updates on service progress  

---

## 4. Non-Functional Requirements  

### 4.1 Performance  
- System must respond to a user query within 3 seconds  
- Voice recognition must complete within 2 seconds  

---

### 4.2 Scalability  
- System must support thousands of users concurrently  
- Must scale automatically during peak usage  

---

### 4.3 Security  
- All user data must be encrypted  
- Aadhaar and documents must be securely stored  
- Only authorized services can access user data  

---

### 4.4 Availability  
- System must be available 24/7  
- Downtime should be minimal  

---

### 4.5 Usability  
- Interface must be simple and voice-first  
- App must be usable by low-literacy users  

---

## 5. Constraints  

- Must operate on AWS infrastructure  
- Must integrate with UMANG and DigiLocker  
- Must support low-bandwidth environments  

---

## 6. Success Criteria  

The system will be considered successful if:
- Users are guided to government schemes first  
- At least 10,000 users are onboarded in the pilot city  
- At least 30% of users use government services instead of paid ones  

---