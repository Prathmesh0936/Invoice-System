# End User Documentation

## Project Overview
This project is a web-based Group, Chain, Brand, Subzone, Estimate, and Invoice Management System built using **React** with **Vite** as the build tool and **Tailwind CSS** for styling. The application is designed for managing business entities, their relationships, and related financial documents in a user-friendly interface.

**Note:** This project is a frontend-only application. All data is stored in the browser's local storage. There is no backend or database integration in this version.

---

## Main Features

### 1. Dashboard
- View summary cards for total Groups, Chains, and Brands.
- See a table of all Chains with their Group, Company, and GSTN details.
- Filter Chains by Group.
- Quick access to add a new Company/Chain.

### 2. Group Management
- List all Groups with search and filter options.
- Add, edit, or soft-delete (deactivate) Groups.
- Prevent deletion if a Group is linked to any Chain.

### 3. Chain/Company Management
- List all Chains/Companies with search and filter options.
- Add, edit, or soft-delete (deactivate) Chains.
- Prevent deletion if a Chain is linked to any Brand.
- Each Chain is associated with a Group and has a GSTN.

### 4. Brand Management
- List all Brands with search and filter options.
- Add, edit, or soft-delete (deactivate) Brands.
- Each Brand is associated with a Chain.

### 5. Subzone Management
- Manage subzones for each Brand (e.g., Marol, Kurla).
- Add, edit, or soft-delete subzones.
- Filter subzones by Brand, Company, or Group.

### 6. Estimate Management
- Create, edit, and delete service estimates for Groups, Chains, Brands, and Zones.
- Each estimate includes service details, units, price per unit, and total.
- Generate invoices directly from estimates.

### 7. Invoice Management
- View, search, edit, and delete invoices.
- Generate new invoices from estimates or manually.
- Each invoice includes details like invoice number, estimate ID, company, service, amount, and date.

---

## Navigation
The sidebar provides quick access to all major sections:
- Dashboard
- Manage Groups
- Manage Chain
- Manage Brands
- Manage Subzones
- Manage Estimates
- Manage Invoices

The header displays the current section and provides a logout link.

---

## Data Storage
- **All data is stored in the browser's local storage.**
- When you add, edit, or delete Groups, Chains, Brands, Subzones, Estimates, or Invoices, the changes are saved locally in your browser.
- **No data is sent to a server or external database.**
- If you clear your browser's storage or switch browsers/devices, your data will be lost.

---

## Limitations
- This application does **not** connect to any backend or database.
- For production use, integration with a backend API and persistent database is required.
- The SQL files in the project are for reference only and are not used by the application.

---

## Getting Started
1. Install dependencies: `npm install`
2. Start the development server: `npm run dev`
3. Open your browser and navigate to the provided local URL (usually `http://localhost:5173/`).

---

## Support
For questions or issues, please contact the project maintainer or refer to the codebase for further details. 