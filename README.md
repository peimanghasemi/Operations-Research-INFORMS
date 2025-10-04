#  Data-Driven Robust Optimization of Team Orienteering for Resilient Emergency Logistics Operations

This repository contains the GAMS implementation of a **tri-objective optimization model** for integrated air-ground emergency logistics under demand uncertainty.  
The model coordinates **drones and ambulances** to improve supply chain resilience, while considering **facility location, regional clustering, and independent routing**.  

---

##  Highlights
- Tri-objective optimization: unmet demand, maximum response time, and total cost (ε-constraint method).  
- **Data-driven uncertainty modeling** using Conservative Support Vector Clustering (CSVC).  
- Application to **emergency blood deliveries in Orange County, California**.  
- Integrates fairness considerations in high-priority regions.  
- Demonstrates trade-offs between robustness, cost, and responsiveness.  

---

##  Project Structure
- `model.gms` → main GAMS model.  
- `data.xls` → input data file (demand, locations, parameters).  
- `results/` → output folder for solutions and reports.  

---

##  Requirements
- [GAMS](https://www.gams.com/download/) installed.  
- **Solver:** Gurobi (for solving large-scale MILP).  
- Input data in Excel format.  

---

##  Running the Model
1. The optimization model is written in GAMS but stored in a text file (`Deterministic.txt`).  
2. To run the model, you can either:
   - Rename `Deterministic.txt` to `Deterministic.gms` and open it in GAMS, or  
   - Open `Deterministic.txt` directly in GAMS IDE and run it.  
3. The model will read the required data from `data.xls` (or other input files).  
4. Results will be generated and saved in the `results/` folder.  

