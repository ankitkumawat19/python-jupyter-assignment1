# python-jupyter-assignment1
A modular console-based Supermarket Billing System built in Python. Features dynamic shopping cart management, automatic quantity updating, tiered discount logic, and formatted itemized receipt generation.
# 🛒 Supermarket Billing System

A beginner-level Python project that simulates a simple supermarket billing system. The program allows users to select products from different categories, enter quantities, add multiple items to a shopping cart, calculate the subtotal, apply tiered discounts, and generate a final itemized receipt.

This project was created as part of my Python learning and practical application in **Business Analytics**.

---

## 📌 Project Overview

The **Supermarket Billing System** is a console-based Python application designed to demonstrate fundamental programming concepts through a practical retail billing workflow.

The user can:
- Select a product category.
- Browse products within that category.
- Specify the desired quantity.
- Add multiple products to the shopping cart.
- Automatically update item quantities if an existing product is selected again.
- Calculate the order subtotal.
- Apply discount tiers based on total purchase value.
- Generate a clean, itemized final bill.

The project is available in both standard Python script (`.py`) and Jupyter Notebook (`.ipynb`) formats.

---

## ✨ Features

- **Multiple Categories:** Browse across 5 distinct grocery sections.
- **Multi-Item Transactions:** Add any number of products in a single run.
- **Dynamic Shopping Cart:** Automatically merges quantities for repeated items without creating duplicate lines.
- **Tiered Discounts:** Rule-based savings calculated automatically against the subtotal.
- **Formatted Receipts:** Clear console output with itemized lines, discounts, and total payable amounts.
- **Input Validation:** Error-handled inputs using `try-except` blocks to prevent crashes from invalid numbers or choices.

---

## 📦 Product Catalog

The system supports items across the following 5 categories:

| Category | Products Available |
| :--- | :--- |
| **1. Dairy Products** | Milk, Curd, Butter, Cheese |
| **2. Grocery Products** | Rice, White Flour, Sugar, Dal, Cooking Oil, Salt, Coffee, Biscuits |
| **3. Bakery Products** | Bread, Bun, Cake |
| **4. Vegetables** | Potato, Onion, Tomato, Carrot |
| **5. Chocolates & Chips** | Dairy Milk, KitKat, Kinder Joy, Bournville, Ferrero Rocher, Lays, Kurkure, Nachos |

---

## 💻 Python Concepts Used

This project applies core procedural Python concepts:
- **Data Structures:** Dictionaries (product catalog, prices) and Lists (cart state).
- **Control Flow:** `if`, `elif`, `else` conditional branching.
- **Loops:** `while` loops for continuous menu interaction; `for` loops for receipt processing.
- **Functions:** Modular design for displaying menus, computing discounts, and printing bills.
- **Exception Handling:** `try-except` blocks for safe numeric input parsing.
- **Formatting:** String formatting for structured currency and tabular receipt output.

---

## 🔄 Program Flow

```text
Select Category ──► Choose Product ──► Enter Quantity ──► Update / Add to Cart
                                                              │
   ┌──────────────────────────────────────────────────────────┘
   ▼
Add More Items? ──(Yes)──► Repeat Selection Loop
   │
 (No)
   ▼
Calculate Subtotal ──► Apply Discount Tier ──► Print Formatted Receipt
