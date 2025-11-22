# Medical Prescription Analyzer – Project Report (Using Streamlit + Google Gemini)

## 1. Introduction

The **Medical Prescription Analyzer** is an **AI-driven application** designed to interpret both **handwritten** and **printed medical prescriptions**. Using **Google Gemini 2.5 Flash**, the system extracts critical information such as **medicine names**, **dosage**, **patient and doctor details**, and **additional notes**. The goal is to make prescription understanding easier, especially for patients who face difficulty reading **medical handwriting** or **medical shorthand**.



## 2. Problem Statement

Medical prescriptions are often difficult to read due to **unclear handwriting**, **abbreviations**, and **inconsistent formats**. Misinterpretation can lead to **incorrect dosage** or improper **medication intake**.

This project aims to solve this issue by converting prescription images into **structured**, **readable**, and **understandable** information.



## 3. Objectives

- Extract **medicines**, **dosage**, **frequency**, and **instructions** from a prescription image  
- Identify **patient name**, **doctor name**, **hospital information**, and **date** (if available)  
- Detect **unclear** or **unreadable text**  
- Provide an **intuitive interface** for uploading images and analyzing them  
- Allow users to ask **additional queries** related to the prescription  



## 4. Technology Stack

### Frontend
- **Streamlit**

### Backend / AI Model
- **Google Gemini 2.5 Flash**

### Libraries
- **Pillow (PIL)**
- **Google Generative AI Python SDK**
- **dotenv**



## 5. System Workflow

1. User uploads a **prescription image** (JPG/JPEG/PNG)
2. Image is converted into **Gemini-friendly format**
3. The **Gemini model** analyzes the image using a **structured prompt**
4. Extracted details are **formatted and returned**
5. User can ask **additional questions** regarding the prescription



## 6. Key Features

- Works with **handwritten** and **printed prescriptions**  
- Extracts **medicine names**, **dosage**, **frequency**, and **instructions**  
- Identifies **patient/doctor details**  
- Flags **unreadable text**  
- Clean, **easy-to-use** Streamlit app  
- Fast response powered by **Gemini**  

## 7. Example Output

**Patient Name:** Amit Verma  
**Doctor:** Dr. R. Sharma  
**Date:** 12-08-2024  

**Medicines:**  
1. **Amoxicillin 500mg** — **1-0-1** (After food)  
2. **Vitamin C 500mg** — **0-1-0**  
3. **Paracetamol** — **1-1-1** (If fever persists)

**Notes:**  
- Drink **plenty of water**  
- Avoid **cold drinks**  
- Some text is **not readable**  



## 8. Limitations

### 1. Handwriting Quality
- Poor or messy **handwriting** may still be difficult for the model to interpret.
- Older or **blurred scans** may produce incomplete results.

### 2. Medical Terminology Variations
- **Drug names** vary across countries and brands.
- Rare medicines or **shorthand notations** may be misunderstood.

### 3. Image Quality Dependency
- **Low-resolution images**, shadows, reflections, or cropped parts reduce accuracy.

### 4. No Medical Validation
- The system extracts information but does **not verify medical correctness**.
- It cannot replace **professional medical advice**.

### 5. Limited Context Understanding
- Overlapping **medicine entries** or notes may be misinterpreted.
- Handwritten **short forms** may be interpreted differently.



## 9. Future Enhancements

### 1. Multi-Language Support
- Add recognition for prescriptions written in **regional languages**.

### 2. OCR + AI Hybrid System
- Combine **traditional OCR** with **AI** for higher handwriting accuracy.

### 3. Drug Database Integration
- Validate medicines with **FDA/WHO drug directories**.  
- Provide **safety alerts**, **side effects**, and **interaction warnings**.

### 4. Automatic Structuring Into JSON
- Return structured **JSON output** for hospital or pharmacy integration.

### 5. Prescription History Tracking
- Allow users to upload **multiple prescriptions** and maintain a **digital record**.

### 6. Mobile App Version
- A **mobile app** for direct prescription image capture.

### 7. Enhanced Image Preprocessing
- **Noise removal**, **sharpness correction**, **text segmentation**.

### 8. Voice-Based Explanation
- Provide **audio explanations** of prescription details for visually impaired users.



## 10. Conclusion

The **Medical Prescription Analyzer** demonstrates how **AI** can significantly enhance **healthcare accessibility** by simplifying prescription interpretation. Although it has limitations, the system lays a strong foundation for future advancements such as **multi-language support**, **drug validation**, and improved **accuracy**.

With continued development, this solution can evolve into a **comprehensive medical assistance tool**.
