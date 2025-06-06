# 🏦 Bank Branch Simulation with AnyLogic

This project simulates customer service dynamics in a **bank branch**, using **agent-based and discrete-event modeling** in *AnyLogic*. It was developed as a final project for the **Simulation course (11.63)** at ITBA during the first semester of 2024.

The main goal is to explore how to **improve service quality** and **minimize waiting times** under real-world constraints such as limited budgets, fixed infrastructure, and unpredictable customer flows.

---

## 🧩 Project Scope

- Simulation of **three main services**:
  - Commercial assistance (consultations)
  - Teller services (cash-based transactions)
  - ATM usage
- Agents include: clients (regular and VIP), employees, ATMs, queueing systems
- Considered variables:
  - Customer arrival rate
  - Employee experience and training
  - ATM maintenance and failure
  - Budget constraints and service costs

---

## 🎯 Objective Function

> **Service Level = Resolved operations / Total clients**

The project aims to maximize this metric while respecting constraints such as:
- Max 8 employees total
- Monthly budget ≤ $6,000 USD
- Limited number of ATMs (cannot be increased)

---

## ⚙️ Model Features

- Built using **AnyLogic Personal Learning Edition**
- Hybrid logic: **agent-based (customers and staff)** + **event-based (failures, transitions)**
- Dynamic assignment of clients to free staff or machines
- Logic for:
  - Reassigning employees between services based on queue load
  - ATM breakdown, repair or replacement
  - Monthly trainings and their impact on staff performance

See model structure and visual logic diagrams in the [report PDF](./Informe+simulación+-+Grupo+5++-+Banco.pdf).

---

## 🧪 Experiments & Optimization

We designed 4 distinct experiments by varying:
- Number of employees per service
- Monthly training frequency
- Annual ATM maintenance

Additionally, we tested a **heuristic** to dynamically reassign employees between services when queues became unbalanced.

📈 Results included:
- Best-performing configuration:  
  4 employees in Commercial, 2 in Teller, 2 monthly trainings, 9 annual ATM maintenances  
- The heuristic showed **no statistically significant improvement**, but may be useful under tighter budget scenarios.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Simulación.pdf` | Slide deck with visual summary of the simulation and results (in Spanish) |
| `Informe-simulación.pdf` | Full written report detailing methodology, logic, experiments, and conclusions (in Spanish) |
| `Entrega-simulacioon.alp` | AnyLogic simulator file (not included here, must be opened with AnyLogic Personal Learning Edition) |

---

## 📝 Note

> This repository includes all core files from the final simulation project.  
> Both PDF files are written in **Spanish**.  
> If you'd like an English summary of the full report, feel free to reach out.

---
