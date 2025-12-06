# 🧮 Who is the Best?  
## Analysis of Mathematical Ranking Methods in Mathematical Olympiads

### **📄 Abstract**  
This project investigates the fairness, stability, and reliability of several mathematical ranking algorithms — including the **Colley method**, **Massey method**, and **Elo rating system** — when applied to real performance data from mathematical Olympiads.  
By implementing these ranking systems in Python and comparing their outputs, this study aims to understand how different mathematical assumptions influence the final ranking of participants and problems.  
The project demonstrates practical skills in data analysis, linear algebra, numerical methods, and algorithmic reasoning.

---

## 🎯 **1. Motivation**

Ranking problems appear everywhere: sports, competitions, machine learning evaluation, website ranking, and academic selection processes.  
Yet different ranking methods can produce **different outcomes** even when using the same data.

This project explores the question:

> **“How much does the choice of ranking algorithm influence who appears to be the ‘best’?”**

Using mathematical Olympiad data, this project evaluates how three established ranking systems behave under identical performance inputs — revealing strengths, weaknesses, and differences in fairness.

---

## ⚙️ **2. Methods Implemented**

### **2.1 Colley Ranking Method**
- Uses linear algebra and a least-squares system  
- Does not rely on margin of victory  
- Produces stable results in small datasets  
- Implemented in: `colley-2024.ipynb`

### **2.2 Massey Ranking Method**
- Based on the point differentials between competitors  
- Sensitive to score margins  
- Good for identifying dominant performances  
- Implemented in:  
  - `massey-2024.ipynb`  
  - `massey-2024-Student research.ipynb` (alternative version)

### **2.3 Elo Rating System**
- Widely used in chess and e-sports  
- Dynamically updates ratings through pairwise interactions  
- Sensitive to ordering of matches  
- Implemented in:  
  - `elo-2024.ipynb`  
  - `eloRankingTuningEndSeason-2.ipynb` (tuned version)

---

## 📁 **3. Repository Structure**

