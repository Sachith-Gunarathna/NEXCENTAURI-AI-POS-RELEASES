# 🚀 NEXCENTAURI AI POS

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Electron](https://img.shields.io/badge/Platform-Electron-47848F.svg?logo=electron)
![React](https://img.shields.io/badge/Frontend-React.js-61DAFB.svg?logo=react)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57.svg?logo=sqlite)

> **Nextuary-AI-POS-Releases** > The Nexcentauri Advanced AI POS System is a robust, modern, offline-first hybrid Point of Sale (POS) software designed primarily for retail environments and grocery stores. 

Built as a desktop application, it ensures high performance, reliability without requiring constant internet, and seamless hardware integration.

---

## 🛠️ Technology Stack

* **Frontend UI:** Built with **React.js** and **Tailwind CSS** for a fast, responsive, and visually appealing user interface. Features native Dark/Light mode support.
* **Desktop Framework:** Packaged using **Electron.js**, allowing it to run natively as a highly optimized Windows application.
* **Database (Offline-First):** Powered by an offline-first **SQLite** backend (`better-sqlite3`), ensuring lightning-fast queries and zero downtime during internet outages.
* **Cloud Sync (Hybrid):** Integrates with **Firebase** and **AWS S3** for background cloud synchronization, secure data backups, and remote SaaS license verification.

---

## 📦 Core Modules & Features

### 1. 🛒 Advanced Point of Sale (POS) Terminal
* **Fast Checkout:** Optimized for speed with barcode scanner support and quick-search functionalities.
* **Payment Methods:** Supports Cash, Card, Credit (Store Credit), and Split payments.
* **Transaction Controls:** Hold carts (pause transactions), void items, refund sales, and apply cashier or system-level discounts.
* **Weight & Scale Integration:** Direct integration with digital scales via serial ports (`serialport` library) to automatically fetch weights for items like vegetables or bulk goods.
* **Secondary Screen:** Includes a dual-display feature to show real-time cart details and branding to the customer during checkout.

### 2. 📦 Comprehensive Inventory Management
* **Item & Batch Tracking:** Manage products by category and brand. Supports multi-batch tracking with exact manufacturing and expiry dates (FEFO ready).
* **Unit of Measure (UOM) Conversion:** A highly advanced UOM system that allows selling sub-units (e.g., deducting 250g from a 50kg bulk sack) with automatic stock deduction and COGS recalculation.
* **Stock Monitoring:** Automated low-stock thresholds and alert reports.
* **Barcode Generation:** Built-in `JSBarcode` support to generate and print custom product labels.

### 3. 🚚 Supplier & GRN (Goods Received Note)
* **Supplier Directory:** Maintain supplier details, contact info, and current payable balances.
* **GRN Processing:** Add new stock seamlessly using GRNs, linking directly to supplier invoices.
* **Supplier Ledger:** Tracks payments made, pending balances, and adjustments.

### 4. 👥 Customer & Loyalty Management
* **Customer Profiles:** Differentiates between Retail, Wholesale, and B2B customers.
* **Credit/Ledger System:** Allows trusted customers to buy on credit, tracks balances against a set credit limit, and records payments via a detailed credit ledger.
* **Loyalty Points System:** Automatically awards points based on purchase value, allowing customers to redeem points on future visits (secured by optional PIN validation).

### 5. 🧑‍💼 Employee, Attendance & Payroll System
* **Role-Based Access (RBAC):** Cashier, Manager, Accountant, Stock Keeper, and Admin roles with restricted UI access.
* **Biometric Attendance:** Integration with fingerprint scanners to accurately log employee clock-in and clock-out times.
* **Automated Payroll:** Automatically calculates daily salaries based on recorded attendance, OT, and base salary rates, eliminating manual HR workloads.

### 6. 📊 Financials, Reporting & Expenses
* **Daily Analytics:** Generates daily sales summaries, total revenue, tax amounts, and payment method breakdowns.
* **Expense Tracking:** Dedicated module to log day-to-day shop expenses (utility bills, petty cash).
* **Profit Reporting:** Tracks Base Price vs. Sale Price to accurately calculate daily profit margins and COGS.

### 7. 🔒 SaaS Licensing & Security
* **Tiered Gating:** Software is protected by a remote SaaS licensing model (Basic, Premium, Deluxe tiers) restricting specific features based on the purchased package.
* **System Locking:** Includes built-in anti-tamper mechanisms, lock screens, and license revocation handling if a subscription expires.
* **Auto-Updater:** Built-in seamless updates via `electron-updater` directly from GitHub releases.

---

### 👨‍💻 Credits
**Lead Developer:** Sachith Gunarathna  
**Company:** NEXCENTAURI

---
*© 2026 nexcentauri. All rights reserved.*
