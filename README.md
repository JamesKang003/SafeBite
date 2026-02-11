# 🥗 SafeBite

**SafeBite** is an intelligent, AI-assisted allergen scanning Android application designed to help users make safer food choices in real time.

Using on-device computer vision and live food database integration, SafeBite scans product barcodes and analyzes ingredient lists to detect potential allergens within seconds — reducing the cognitive load and risk involved in manual label reading.

---

## 📱 Features

- 📸 **Real-Time Barcode Scanning**  
  Utilizes **Google ML Kit** with **CameraX** to perform fast, on-device barcode recognition with low latency and high accuracy.

- 🧠 **Automated Allergen Detection Engine**  
  Fetches product data via the **FatSecret API**, parses ingredient lists, and programmatically matches against known allergen categories (e.g., peanuts, dairy, gluten, soy).

- ⚡ **Asynchronous API Handling**  
  Implements non-blocking network requests to maintain smooth UI performance while retrieving and processing remote data.

- 🎨 **Modern Declarative UI**  
  Built entirely using **Jetpack Compose**, enabling reactive UI updates and modular component design.

- 🧩 **Structured Architecture (MVC-inspired)**  
  Separates concerns between:
  - **Model** → API data models & allergen logic  
  - **View** → Compose UI components  
  - **Controller / Logic Layer** → Barcode processing, API orchestration, data parsing  

- 🔍 **Ingredient Parsing & Normalization**  
  Handles inconsistent API formatting by cleaning and standardizing ingredient strings before allergen comparison.

- 🔐 **Privacy-Focused Design**  
  Barcode recognition runs on-device using ML Kit, reducing dependency on external vision services.

- 🗂️ **Version Control & Iterative Development**  
  Managed using Git & GitHub with structured commits and modular code organization.

---

## 🧰 Tech Stack

| Category | Tools / Frameworks |
|-----------|--------------------|
| Language | Kotlin |
| UI Framework | Jetpack Compose |
| Architecture | MVC (Model–View–Controller) |
| Computer Vision | Google ML Kit |
| Camera API | CameraX |
| Networking | Retrofit / HTTP Client |
| Data Format | JSON |
| API | FatSecret API |
| IDE | Android Studio |
| Build System | Gradle |
| Version Control | Git, GitHub |

---

## 🔄 System Workflow

1. User launches SafeBite  
2. Camera scans product barcode using ML Kit  
3. Barcode ID is extracted on-device  
4. App sends secure API request to food database  
5. Ingredient list is retrieved and parsed  
6. Allergen detection engine matches ingredients against known allergen patterns  
7. UI dynamically updates with flagged allergens  

Average scan-to-result time: a few seconds depending on network conditions.

---

## 🧠 Engineering Challenges Solved

- Integrating real-time camera input with ML inference  
- Managing asynchronous API calls without blocking UI  
- Handling inconsistent ingredient string formats  
- Designing modular UI components with Compose  
- Maintaining separation of concerns for scalability  

---

## 📌 What This Project Demonstrates

- Applied AI integration in mobile applications  
- End-to-end feature ownership  
- API orchestration & data transformation  
- Clean architecture and modular design  
- User-focused risk mitigation through software  

---

## 🚀 Future Improvements

- Custom user-defined allergen profiles  
- Offline ingredient caching  
- OCR-based ingredient label scanning (text recognition)  
- Nutrition scoring and recommendation engine  
- Cloud-based personalization layer  

---
