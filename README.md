# BudgetBuddy — Classical Ledger Expense & Budget Tracker

A feature-rich, modular personal finance ledger and expense management web application. Built with a classical ledger green & warm gold aesthetic, combining pure semantic HTML5, CSS3, modular JavaScript, and modern **React 19** interactive components.

---

## 🌟 Key Highlights

- **Classical Ledger Design**: Deep ledger green (`#16382c`), warm gold (`#c99a3b`), and parchment paper (`#f6f4ee`) visual theme inspired by physical accounting journals.
- **⚛️ React 19 Interactive Suite**:
  - `<QuickExpenseLogger />`: Controlled inputs with preset chips (`+₹100`, `+₹250`, etc.) and bi-directional storage synchronization.
  - `<BudgetSimulator />`: Real-time "What-If" spending slider with dual-fill progress meters and deficit alerts.
  - `<ReactHealthDashboard />`: Live category distribution percentages and net retention analytics.
  - **React Lab Tab**: Dedicated full-screen interactive financial lab workspace.
- **Modular 3-Tier Architecture**: 12 dedicated JavaScript modules with clean separation of concerns and team ownership.
- **Dual-Role Dashboards**: Role-based access control separating **Standard Users** (personal expense management) and **Faculty Administrators** (system statistics, user management, audit logs).
- **Persistent Local Storage**: Complete offline data persistence in `localStorage` with rich pre-seeded records for instant evaluation.
- **Multi-Account Reconciliation**: Supports Cash, Bank, UPI / GPay, and Credit Card accounts with automatic double-entry balance adjustment.
- **Native Data Export**: Built-in CSV export, printer-ready financial report generation, and JSON database backup/restore.

---

## 👥 3-Member Team Work Allocation

| Team Member | Role | Assigned Modules | Primary Technical Contributions |
| :--- | :--- | :--- | :--- |
| **Member 1** | Data Architect & Security Engineer | `js/storage.js`<br>`js/auth.js`<br>`js/admin.js`<br>`js/settings.js` | LocalStorage Engine, Schema Migrations, Session Lifecycle, RBAC Security, Audit Logging, Theme & JSON Backup Engine |
| **Member 2** | Financial Logic & Ledger Systems Engineer | `js/transactions.js`<br>`js/accounts.js`<br>`js/budget.js`<br>`js/recurring.js` | Double-Entry Reconciliation, Multi-Account Balancer, Filter Engine, Budget Variance Math, Recurring Bill Scheduler |
| **Member 3** | Frontend Lead & React Specialist | `js/react-components.js`<br>`js/analytics.js`<br>`js/user.js`<br>`js/app.js` | React 19 Hooks (`useState`, `useMemo`), SPA Tab Router, Interactive What-If Simulator, Financial Health Visualization |

> Detailed documentation and viva presentation scripts are available in [**`TEAM_CONTRIBUTIONS.md`**](TEAM_CONTRIBUTIONS.md).

---

## 📂 Project Structure

```
budgetbuddy/
├── index.html                     # Main Single-Page Application interface with 9 views & modals
├── style.css                      # Classical ledger green & gold design system with Dark Mode
├── presentation.html              # Interactive 8-slide presentation deck (runnable in browser)
├── BudgetBuddy_Presentation.pptx  # 8-Slide PowerPoint Presentation for evaluations
├── TEAM_CONTRIBUTIONS.md          # Team member work allocation & viva speaking scripts
├── README.md                      # Project documentation
├── package.json                   # Node.js project manifest & scripts
├── server.js                      # Lightweight zero-dependency local HTTP server
├── build_browser_react.js         # React 19 browser runtime compilation script
├── generate_ppt.js                # PowerPoint generator script
└── js/
    ├── vendor/
    │   └── react-browser-bundle.js # Self-contained offline React 19 & ReactDOM runtime
    ├── react-components.js        # React 19 Component Suite: Simulator, Quick Logger, Health
    ├── storage.js                 # Database Layer: localStorage persistence & seed data
    ├── auth.js                    # Module 1: 🔐 Authentication & Role Management
    ├── user.js                    # Module 2: 👤 User Financial Aggregation
    ├── transactions.js            # Module 3: 💸 Expense & Income Management
    ├── accounts.js                # Module 4: 🏦 Account & Category Management
    ├── budget.js                  # Module 5: 💰 Budget Variance & Limit Engine
    ├── recurring.js               # Module 6: 🔄 Recurring Expense Management
    ├── analytics.js               # Module 7: 📊 Analytics & Reports
    ├── admin.js                   # Module 8: 🛡️ Admin Console & Audit Logs
    ├── settings.js                # Module 9: ⚙️ Settings, Dark Mode & Backup/Restore
    └── app.js                     # SPA Orchestrator: Tab routing, modals & toast alerts
```

---

## 🔑 Demo Credentials for Faculty Evaluation

The login page features **1-Click Quick Demo Buttons** for instant evaluation:

| Role | Email | Password | Access Level |
| :--- | :--- | :--- | :--- |
| **Demo User** | `user@budgetbuddy.com` | `user123` | Personal Dashboard, Ledger, Budgets, Recurring Bills, React Lab, Analytics |
| **Faculty Admin** | `admin@budgetbuddy.com` | `admin123` | Admin Console, User Control, System Metrics, Global Audit Logs |

---

## 🚀 How to Run

### Method 1: Double-Click (No Install Needed)
Double-click `index.html` in Windows File Explorer. It opens instantly in your default web browser (Edge, Chrome, Firefox) with 100% offline functionality.

### Method 2: Local HTTP Server (Node.js)
```bash
node server.js
```
Then navigate to **http://localhost:3000** in your browser.

---

## 📑 Presentation & Slide Deck

- **PowerPoint**: Open [`BudgetBuddy_Presentation.pptx`](BudgetBuddy_Presentation.pptx) in Microsoft PowerPoint or Google Slides.
- **Browser Deck**: Open [`presentation.html`](presentation.html) in any browser for an interactive 16:9 presentation with arrow-key navigation.
