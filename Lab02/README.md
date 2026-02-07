# Lab 02: Student Performance Prediction

## 1. Dataset Selection

**Dataset Name:** Student Performance Data Set  
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance)  
**Data File:** `student-mat.csv` (Math course performance)

## 2. Problem Definition

Based on the dataset analysis, the machine learning problem is defined as follows:

* **Problem Type:** **Regression**
  * *Reasoning:* We are predicting a continuous numerical value (the final grade, ranging from 0 to 20), rather than a categorical class.
* **Target Variable:** `G3`
  * *Description:* The final grade (ranging from 0 to 20).
* **Goal:** The model is expected to learn the relationship between a student's personal/social factors and their academic performance to predict their final score (`G3`).

## 3. Problem Description

The goal of this project is to build a machine learning model that predicts the academic performance of students in secondary education (specifically in Mathematics).

Using a dataset of 395 students from two Portuguese schools, the model will analyze various demographic, social, and school-related features. These features include the student's home environment (e.g., parents' education `Medu`/`Fedu`, family size `famsize`), study habits (`studytime`, `failures`), and social behaviors (e.g., alcohol consumption `Walc`/`Dalc`, free time `freetime`).

The core objective is to determine if these background factors, combined with earlier grades (`G1` and `G2`), can accurately forecast a student's final grade (`G3`). This analysis could help educators identify students at risk of failure early in the academic year.

## 4. Key Attributes

The dataset contains **33 attributes**. Some of the most significant features used for prediction include:

* **School & Demographics:** `school`, `sex`, `age`, `address`.
* **Family Background:** `Pstatus` (parent cohabitation status), `Medu`/`Fedu` (mother/father education), `Mjob`/`Fjob` (parents' jobs).
* **Academic History:** `failures` (past class failures), `schoolsup` (extra educational support), `absences`.
* **Lifestyle:** `goout` (going out with friends), `Dalc`/`Walc` (workday/weekend alcohol consumption), `health` (current health status).
* **Grades:**
  * `G1`: First period grade (0-20)
  * `G2`: Second period grade (0-20)
  * `G3`: Final grade (Target Variable, 0-20)

## 5. Methodology

The following diagram outlines the machine learning workflow for this project:

![Methodology Diagram](Methodology%20Diagram.png)
