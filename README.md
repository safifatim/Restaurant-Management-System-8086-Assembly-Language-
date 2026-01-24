# 🍽️ Restaurant Management System (8086 Assembly)

![Language](https://img.shields.io/badge/Language-8086%20Assembly-orange)
![Env](https://img.shields.io/badge/Environment-DOSBox-blue)
![Architecture](https://img.shields.io/badge/Architecture-16--bit%20Real%20Mode-lightgrey)

An interactive, console-based management system developed in **8086 Assembly Language**. [cite_start]This project demonstrates low-level software engineering, direct hardware interaction, and manual memory management within the **DOS environment**[cite: 1, 3].

---

## 🚀 Overview
[cite_start]The system provides a complete workflow for restaurant operations, including category navigation, item selection, and automated billing[cite: 1, 4]. [cite_start]It is built to showcase the practical implementation of assembly concepts like macros, procedures, and interrupt-level I/O[cite: 1, 2].



## 🛠️ Key Technical Features
* **Interrupt-Driven UI:** Uses `INT 21h` for string output/input and `INT 10h` for BIOS-level screen clearing.
* **Modular Design:** Implements **Macros** for repetitive print tasks and **Procedures** for complex logic like numeric conversion.
* **Register-Level Logic:** Utilizes the `BX` register as a base pointer to navigate word arrays containing item prices.
* **Custom Arithmetic Module:** Calculates totals using the formula:
    $$Total = \sum (Price \times Quantity)$$
* **Number Printing Procedure:** A custom algorithm that converts binary values to ASCII digits using stack operations.

## 📋 System Menu & Pricing
The system manages 5 distinct categories with 8 items each. 

| Category | Sample Items | Price Range (PKR) |
| :--- | :--- | :--- |
| **Breakfast** | Paratha, Omelette, Halwa | [cite_start]10 - 30 [cite: 8, 9] |
| **Lunch** | Chicken Biryani, Kabab, Salad | [cite_start]20 - 180 [cite: 9, 10] |
| **Dinner** | Makhni Handi, Beef Curry, BBQ Rice | [cite_start]30 - 170 [cite: 10, 11] |
| **Snacks** | Shawarma, Burgers, French Fries | [cite_start]10 - 130 [cite: 11, 12] |
| **Drinks** | Mineral Water, Juices, Lacchi | [cite_start]15 - 100 [cite: 12, 13] |

## 💻 How to Run
1.  Install **DOSBox**.
2.  Mount your project directory.
3.  Assemble and Link (if using source) or run the executable directly:
    ```bash
    COAL_PROJECT_FINAL.exe
    ```

## ⚠️ Limitations & Future Scope
* [cite_start]**Current:** Runs in 16-bit Real Mode only; no external file storage[cite: 8].
* [cite_start]**Future:** Planned support for item-wise billing, discount functionality, and graphical interfaces[cite: 9].

## 🤝 Contributors
* **[Your Name]** - System Architecture & Core Logic
* **@[Friend's Name]** - [Contribution Area]
* **@[Friend's Name]** - [Contribution Area]

---
*Developed as a final project for the Computer Organization and Assembly Language (COAL) course.*
