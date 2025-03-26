# FCFS Scheduler

This repository contains a clean, practical implementation of the First-Come, First-Served (FCFS) scheduling algorithm - one of the fundamental process scheduling methods in operating systems. Developed during my foundational bootcamp experience, this project not only demonstrates core OS concepts but also serves as an excellent example of sequential process management.

---

## 📌 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Project Structure](#project-structure)
- [License](#license)
- [Contact](#contact)

---

## 🖥️ Introduction

In many systems, processes are queued based on their **arrival times**. The **First-Come, First-Served (FCFS)** scheduling algorithm ensures that each process is executed in the exact order it arrives. This approach helps in understanding **CPU scheduling fundamentals** and analyzing key performance metrics such as **waiting time** and **turnaround time**.

This project **simulates FCFS scheduling**, allowing users to visualize execution order, compute scheduling metrics, and generate a **Gantt chart** for better process tracking.

---

## ⭐ Features

- **Process Simulation:** Models process execution in an FCFS manner.
- **Queue Visualization:** Displays how processes enter and exit the ready queue.
- **Metrics Computation:** Calculates:
  - **Waiting Time:** Time spent in the queue before execution.
  - **Turnaround Time:** Total time from arrival to completion.
  - **Response Time:** The time between arrival and first execution.
- **Gantt Chart Visualization:** Generates a **graphical representation** of process execution.
- **User Input Support:** Allows dynamic input of process details.

---

## ⚙️ Installation

To set up the project, follow these steps:

 ### **Step 1: Clone the Repository**
Clone this repository to your local machine using:

```bash
git clone https://github.com/dxi7/FCFS-Scheduler.git
```
 ### **Step 2: Navigate to the Project Directory**
Once the cloning process is complete, move into the project directory:

```bash
cd FCFS-Scheduler
```
 ### **Step 3: Install Dependencies**
Install the required Python libraries:

```bash
pip install tabulate matplotlib
```
These libraries are used for displaying tables and generating Gantt charts.

---
## 🚀 Usage
To run the program, execute the following command:

```bash
python src/FCFS_Scheduling.py
```
### **User Input**
**The program will prompt you to enter the following details:**

  - **Number of processes**

  - **Arrival time of each process**

  - **Burst time (execution duration) of each process**

**Once the input is provided, the program will display:**

  - **A detailed process table with execution times.**

  - **Average waiting, turnaround, and response times.**

   - **A Gantt chart to visualize the execution order.**
---
## 🔍 Methodology
 ### **Algorithm Overview**
  - **The FCFS scheduling algorithm sorts processes by arrival time.**

  - **The CPU executes each process sequentially, completing one before starting the next.**

  ### **Key Scheduling Metrics:**

  - **Waiting Time (WT): Time spent waiting in the queue before execution.**

   - **Turnaround Time (TAT): Total time from process arrival to completion.**

  - **Response Time (RT): Time from process arrival to the first execution.**
---
## 📂 Project Structure
```bash
FCFS-Scheduler/
├── notebooks/
│   ├── Example_Analysis.ipynb  # Jupyter notebook for demonstrations
├── src/
│   ├── FCFS_Scheduling.py      # Main implementation of FCFS algorithm
├── LICENSE
├── README.md
```
 ### **Directory Breakdown**
   - **notebooks/ → Jupyter notebooks for algorithm analysis.**

   - **src/ → The main Python script implementing FCFS.**

   - **LICENSE → Defines licensing terms.**

   - **README.md → Project documentation.**
---
## 📊 Example Output
### **Process Table:**
**After entering the process details, the program will output the following table:**

```plaintext
+------------+--------------+------------+-----------------+-----------------+--------------+---------------+
| Process ID | Arrival Time | Burst Time | Completion Time | Turnaround Time | Waiting Time | Response Time |
+------------+--------------+------------+-----------------+-----------------+--------------+---------------+
|     P4     |      0       |     8      |        8        |        8        |      0       |       0       |
|     P3     |      2       |     6      |       14        |       12        |      6       |       6       |
|     P2     |      4       |     5      |       19        |       15        |     10       |      10       |
|     P5     |      6       |     4      |       23        |       17        |     13       |      13       |
|     P1     |      7       |     4      |       27        |       20        |     16       |      16       |
+------------+--------------+------------+-----------------+-----------------+--------------+---------------+
```
### **Process Averages:**
**Here are the computed averages for the processes:**

```plaintext
+-------------------------+---------+
| Metric                  |   Value |
+=========================+=========+
| Average Waiting Time    |     9   |
+-------------------------+---------+
| Average Turnaround Time |    14.4 |
+-------------------------+---------+
| Average Response Time   |     9   |
+-------------------------+---------+
```
### **Gantt Chart:**
**The following Gantt Chart clearly shows the execution order of the processes:**

![image](https://github.com/user-attachments/assets/5abeb670-5401-45c2-b049-5f05d8f8865c)

---
## 📜 License
**This project is licensed under the MIT License. You are free to use, modify, and distribute the code following the license terms.**

---
## 📩 Contact
For questions or suggestions, feel free to reach out:

- **Name:** Dina Almutairi  
- **Email:** [dina.almutairi@gmail.com](mailto:dina.almutairi@gmail.com)  
- **LinkedIn:** [Dina Almutairi](https://www.linkedin.com/in/dina-almutairi)
