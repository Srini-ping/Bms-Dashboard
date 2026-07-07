# BMS Monitoring & Maintenance Dashboard

A comprehensive, standard HTML/CSS/JS Building Management System (BMS) dashboard designed for the P.G. Senapathy Centre for Computing Resources (IIT Madras). This centralized platform provides a professional, modern interface for monitoring and managing critical electrical infrastructure, tracking facility maintenance, and visualizing hardware performance trends.

## 🚀 Features

* **UPS System Monitoring:** Select and track individual UPS units (e.g., 200kVA Socomec, 30kVA Delta). Supports manual data entry for kVA, percentage, or Amps per phase (L1, L2, L3) with automated load calculations.
* **Power Distribution (EB1 & EB2):** Monitor main source panels, calculate real-time kVA based on R, Y, B amps, and track total kWh consumption.
* **Hardware Maintenance Scheduler:** A dedicated module to track the lifecycle of facility equipment (UPS, Battery Banks, AHUs). Manages Date of Installation, AMC (Annual Maintenance Contract) periods, Last PM (Preventive Maintenance) dates, and auto-calculates Next PM dates. 
* **HVAC & DG Set Logging:** Track chiller/pump running statuses, monitor multi-zone temperature/humidity, and log DG set running hours, fuel levels, and kVA loads.
* **Advanced Data Visualization:** Master trend dashboards using Chart.js to visualize historical data (All-time, 7-day, 30-day filters) across Line and Bar charts.
* **Data Export & Cloud Sync:** Export module data directly to CSV (spreadsheet) format. Includes a built-in function to sync all locally saved records to a Google Drive spreadsheet via Google Apps Script.
* **Role-Based Access Control:** Secure admin mode to manage operators, lock sensitive maintenance data edits, and generate global reports.

## 🛠️ Tech Stack

* **Frontend:** Standard HTML5, CSS3 (Modern, professional UI with a Dark Blue & Light Gray color scheme).
* **Logic:** Vanilla JavaScript (No React or heavy frameworks).
* **Charting:** Chart.js (via CDN) for dynamic graph rendering.
* **Storage:** LocalStorage for immediate data retention, with Google Sheets webhook integration.

## 📂 Project Structure

The entire application is self-contained for easy deployment and modification:

* `index.html` - Contains all markup, modular CSS styling, and JavaScript logic for rendering UI components, handling calculations, and exporting data.

## ⚙️ Installation & Usage

1.  **Clone the repository:**
    git clone https://github.com/yourusername/bms-dashboard.git
    
2.  **Run the application:**
    Since this is built with standard HTML, simply open the `index.html` file in any modern web browser. No local server or build tools are required.
3.  **Google Sheets Integration (Optional):**
    To enable the "Sync to Google Sheets" feature, replace the `GOOGLE_APP_SCRIPT_URL` variable in the `<script>` section with your own Google Apps Script Web App URL.

## 🔐 System Access

* **Operator Mode:** Select an operator from the login dropdown to begin logging routine data.
* **Admin Mode:** Click "Admin Access" on the login screen. 
    * *Default ID:* `ccprj44`
    * *Default Password:* `12345`

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the issues page if you want to contribute.

## 📄 License

This project is created for the P.G. Senapathy Centre for Computing Resources - IIT Madras.
