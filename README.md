# 💵 Cash Register

A simple and interactive **cash register web application** that lets users select products, enter the cash tendered by the customer, and calculates the correct change due. It also maintains and updates the **cash-in-drawer (CID)**, simulating a real-world cash register system.

Example: [Live Demo](https://cash-register-chi.vercel.app/)

## 📋 Project Overview

This project mimics the core functionality of a point-of-sale (POS) register:

- Users select a product with a set price  
- Input the amount of cash received  
- The app calculates the **change due** using the available denominations in the drawer  
- It handles edge cases like **exact change** or **insufficient funds**  
- Dynamically updates the **cash drawer status**


## 🛠 Technologies Used

- **HTML5**
- **CSS3**
- **JavaScript**


## 📁 Project Structure
```
CashRegister/
├── index.html # Main HTML structure
├── styles.css # CSS for layout and styling (optional)
├── script.js # JavaScript for logic and dynamic UI
└── README.md # This documentation file
```


## 🔍 How It Works

1. Cash-in-drawer is stored as an array with:
   - Denomination names  
   - Corresponding amount in dollars
2. All calculations are performed in **cents** to avoid floating-point issues.
3. The algorithm:
   - Iterates from **largest to smallest** denominations  
   - Dispenses maximum possible of each denomination without exceeding change due
4. Statuses:
   - ✅ **OPEN**: Change given and drawer still has money left  
   - 🔒 **CLOSED**: Drawer is empty after transaction  
   - ❌ **INSUFFICIENT_FUNDS**: Not enough change to complete the transaction


## 📌 Notes

This project is part of the freeCodeCamp [JavaScript Algorithms and Data Structures Certification](https://www.freecodecamp.org/certification/DenXDev/javascript-algorithms-and-data-structures-v8).
It fulfills the requirements for the "Build a Cash Register" project challenge.

