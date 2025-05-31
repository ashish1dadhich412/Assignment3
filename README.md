# 📄 README

## 🏗️ Project Setup

This project contains test cases for the **Login feature** (for example, Amazon/Flipkart) designed using three test case design techniques:

✅ Equivalence Partitioning (EP)  
✅ Boundary Value Analysis (BVA)  
✅ Decision Table

The deliverable is provided as a **document (or spreadsheet)** with clearly labeled sections for each technique.

---

## 🛠️ Build Commands

There are no build or run commands for this assignment because it focuses purely on test design documentation, not executable code.

However, if you want to organize this in a repository, you can structure it like:


---

## ⚙️ Brief Description of Functionalities

The document includes the following test designs for the **Login feature**:

---

### 1️⃣ Equivalence Partitioning (EP)

| Test Case ID  | Input Type       | Test Data                  | Expected Result                |
|---------------|------------------|----------------------------|--------------------------------|
| EP_TC_01      | Valid email      | user@example.com           | Login successful               |
| EP_TC_02      | Invalid email    | user@com                  | Error: invalid email format    |
| EP_TC_03      | Empty password   | user@example.com + ‘’      | Error: password required       |
| EP_TC_04      | Invalid password | user@example.com + 123     | Error: incorrect password      |

---

### 2️⃣ Boundary Value Analysis (BVA)

| Test Case ID  | Boundary Type      | Test Data                  | Expected Result                                |
|---------------|--------------------|----------------------------|------------------------------------------------|
| BVA_TC_01     | Min email length   | a@b.c                     | Login successful                               |
| BVA_TC_02     | Max email length   | [255-char-email]          | Login successful or trimmed                   |
| BVA_TC_03     | Min password len   | 6 characters              | Login successful if valid                    |
| BVA_TC_04     | Max password len   | 20 characters             | Login successful if valid                    |

---

### 3️⃣ Decision Table

| Condition                        | Action                            |
|----------------------------------|----------------------------------|
| Valid email + valid password     | Login successful                 |
| Invalid email + any password     | Show error: invalid email        |
| Valid email + empty password     | Show error: password required    |
| Valid email + wrong password     | Show error: incorrect password   |

---

✅ **Submission:**  
Please submit your GitHub repository link containing:
- This README file.
- The document/spreadsheet with all test cases.



