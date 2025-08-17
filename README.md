## 🏥 Master Patient Indexing (MPI)  

Developed a **Master Patient Indexing system** to create a **single unified patient record** by consolidating data from multiple clinical and demographic sources.  
The system ensured accurate patient identification, reduced duplication, and improved continuity of care across healthcare providers.  

---

### 📌 Background & Problem  
Healthcare organizations often deal with **fragmented patient records** spread across different systems (labs, hospitals, insurance).  
- Duplicate or mismatched records cause **errors in treatment**.  
- Patient identity inconsistencies (e.g., name variations, address changes) lead to **inefficient care coordination**.  
- Existing systems lacked robust **record-linking algorithms** that balance accuracy and scalability.  

This project aimed to build an MPI solution that ensures **reliable, secure, and scalable patient identity management**.  

---

### 🎯 Objectives  
- Consolidate patient data from multiple hospital and clinic systems.  
- Detect and resolve **duplicate/mismatched records**.  
- Create a **unified patient ID** for each individual.  
- Ensure compliance with **healthcare data privacy regulations** (HIPAA).  
- Provide APIs for **secure querying and integration** into healthcare platforms.  

---

### ⚙️ Solution Approach  
1. **Data Collection & Standardization**  
   - Integrated clinical + demographic data from multiple hospital databases.  
   - Applied data cleaning and normalization (standardized DOB formats, address matching, etc.).  

2. **Record Matching Algorithms**  
   - Used **deterministic matching** (exact matches on identifiers such as SSN, MRN).  
   - Applied **probabilistic & fuzzy matching** (similarity scoring on names, addresses, phone numbers).  

3. **Unique Patient Identifier (UPI)**  
   - Assigned a consolidated patient ID once confidence thresholds were met.  
   - Stored mappings to allow backward traceability.  

4. **API Development**  
   - Built **Flask-based services** for querying and updating patient records.  

5. **Database Layer**  
   - Deployed on **MongoDB** to handle scalable, document-oriented patient records.  

---

### 🛠️ Tech Stack  
- **ML & Matching:** Scikit-learn (similarity scoring), Fuzzy Matching libraries  
- **Backend:** Flask  
- **Database:** MongoDB  
- **Compliance:** HIPAA  
- **Language:** Python 3.x  

---

### 📊 Results & Impact  
- Reduced duplicate patient records by **>40%**.  
- Improved accuracy of **patient identity resolution**.  
- Ensured **seamless data integration** across multiple hospital systems.  
- Enhanced **patient safety** by minimizing risks from mismatched records.  

---

### 🚀 Future Enhancements  
- Implement **graph-based record linkage** for more complex relationships.  
- Integrate **biometric identifiers** (fingerprint, facial recognition) for higher accuracy.  
- Deploy on **cloud infrastructure (AWS/Azure/GCP)** for scalability.  
- Add **real-time patient matching APIs** for hospital EMR/EHR systems.  

---

### 📌 Note  
This project was implemented in a **healthcare data integration setting**.  
Due to confidentiality, datasets and code cannot be shared — this description serves as a **case study of applied healthcare data engineering + ML**.  

---
