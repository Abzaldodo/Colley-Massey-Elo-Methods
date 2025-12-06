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
  - `massey-2024-Student research.ipynb` (Analyzing students specifically)

### **2.3 Elo Rating System**
- Widely used in chess and e-sports  
- Dynamically updates ratings through pairwise interactions  
- Sensitive to ordering of matches  
- Implemented in:  
  - `elo-2024.ipynb`  

---

## 📁 **3. Repository Structure**
/
├── All olympiads 2024.csv # Main dataset of Olympiad results
├── data formatting.ipynb # Data cleaning & preparation
├── colley-2024.ipynb # Colley ranking implementation
├── massey-2024.ipynb # Massey ranking implementation
├── massey-2024-Student research.ipynb # Analysis of specifically student performance
├── elo-2024.ipynb # Elo ranking implementation
├── eloRankingTuningEndSeason-2.ipynb # Tuning constant K for best Elo performance
│
├── Problem ranking COLLEY # Output: Colley rankings for Math Olympiad Problems
├── Problem ranking Massey # Output: Massey rankings for Math Olympiad Problems
├── Problem ranking ELO # Output: Elo rankings for Math Olympiad Problems
│
├── 24games.txt # All Student vs Problem games
├── 24teams.txt # Indexes of all students and problems
├── 24points.txt # Points each contestant earned from each problem
│
└── README.md # Project documentation
---


---

## 📊 **4. Workflow**

1. **Data Preparation**  
   - Open `data formatting.ipynb`  
   - Clean raw data  
   - Prepare matrices for ranking algorithms  

2. **Apply Ranking Algorithms**  
   - Run the appropriate notebook (Colley, Massey, or Elo)  
   - The notebooks compute the ranking vectors using:  
     - linear systems (`Ax = b`)  
     - iterative updates  
     - scoring differentials  

3. **Analyze and Compare**  
   - Check how participant or problem rankings shift  
   - Compare stability between methods  
   - Study algorithm sensitivity  

---

## 📝 **5. Results & Observations**

Although detailed results are in the output files, the general findings include:

- **Colley method** produces the most **stable** rankings with minimal sensitivity to score differences.  
- **Massey method** reacts strongly to large score gaps, which can push outlier performances high in ranking.  
- **Elo system** depends heavily on match sequence and allows dramatic rating movements in early rounds.  

This demonstrates that **“best performer” is not absolute** — it depends on the mathematical framework used.


---

## 🚀 **6. Future Extensions**

Possible next steps include:

- Adding **PageRank**-style random-walk ranking  
- Applying **Bayesian ratings** (e.g., TrueSkill)  
- Visualizing ranking transitions using plots  
- Running analysis across multiple years of Olympiad data  
- Creating an interactive dashboard to explore ranking methods  

---

## 📫 **7. Contact**

Author: **Abzal Tangsykbay**  
For academic or research inquiries, feel free to reach out through GitHub.

---

