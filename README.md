# 🚢 Maersk Container Transportation Optimization

**Mixed-Integer Linear Programming model achieving 46% cost reduction in Turkey's logistics network**

## 🎯 Project Overview
Optimization model for Maersk's container transportation network, focusing on maximizing fixed fleet utilization while minimizing transportation costs. Developed as part of Carnegie Mellon University MSBA capstone project.

**Team:** Anup Jain, Nivedha Raj, Ayush Kumar, Poorvi Phulwani  
**Faculty Advisor:** Brad Runyon, Prof. Ganesh Mani  

## 🚀 Key Results
| Metric | Baseline | Optimized | Improvement |
|--------|----------|-----------|-------------|
| **Total Cost** | $4,207,163 | $2,257,717 | **46% reduction** |
| **Fixed Fleet Usage** | 10% | 22% | **120% increase** |
| **3PL Dependency** | 90% | 78% | **13% reduction** |
| **Annual Savings** | - | - | **$1.95M** |

## 🛠️ Technical Implementation
- **Programming:** Python, Gurobi Optimizer
- **Model Type:** Mixed-Integer Linear Programming (MILP)
- **Data Scale:** 22,899 shipments across 1,397 routes
- **Planning Horizon:** 7-day tactical optimization

## 📊 Business Problem
**Challenge:** Manual truck assignment decisions led to:
- Only 10% utilization of fixed fleet assets
- 90% dependency on costly 3PL providers
- No optimization logic in transportation planning

**Solution:** MILP model optimizing truck assignments with constraints:
- Fleet capacity (18 fixed trucks)
- Driver hours-of-service (8 hours/day max)
- Container compatibility requirements
- 15% cost advantage for fixed fleet vs 3PL

## 🏗️ Model Architecture
The optimization model (`maersk_optimization_model.py`) includes:
- **Data preprocessing** and validation
- **MILP formulation** with Gurobi solver
- **Constraint handling** for real-world business rules
- **Results analysis** and visualization
- **Sensitivity testing** across demand scenarios

## 📈 Business Impact
- **Strategic Implementation:** Framework now used in Maersk's strategic planning
- **Scalability:** Model tested up to 50,000+ shipments
- **ROI:** 300%+ return on investment
- **Robustness:** ±7% performance across 10 demand scenarios

## 🔒 Data Privacy
This repository contains the optimization model and methodology. Actual Maersk data is confidential and not included for privacy reasons.

## 📄 Files
- `maersk_optimization_model.py`: Complete optimization model implementation
- `final_presentation.pdf`: Executive presentation with results and methodology
- `data/README.md`: Data structure description (no actual data)

## 🏆 Recognition
- Presented to Maersk C-suite executives
- Selected for Future Leaders Program
- 95% stakeholder approval on recommendations
- Framework adopted for strategic planning across $45B operations
