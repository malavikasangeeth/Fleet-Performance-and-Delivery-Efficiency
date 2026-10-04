# Power BI Analytics Dashboard

An interactive Power BI report designed to analyze supply chain, shipping metrics, fuel/gas consumption, and financial performance.

---

## 📌 Project Overview

This Power BI repository contains data models, custom themes, visual layouts, and embedded media assets configured to deliver executive-level analytics across core operational metrics:

- **Financial Analytics**: Tracking revenue, costs, and dollar-denominated performance indicators.
- **Logistics & Shipping**: Analyzing shipping durations, delivery timelines, and logistics performance.
- **Fuel & Resource Management**: Monitoring gas/fuel consumption, fuel efficiency, and related operational expenses.

---

## 📁 Repository & File Structure

```text
├── DataModel                                  # Compressed VertiPaq tabular data model schema & logic
├── DiagramLayout                              # Power BI Relationship view layout configuration
├── Metadata                                   # Dataset and model metadata attributes
├── Settings                                   # Report-level configurations and parameters
├── SecurityBindings                           # Data access and security configurations
├── [Content_Types].xml                        # OPC package manifest
└── Report/
    ├── Layout                                 # JSON layout definition for visual canvases & pages
    └── StaticResources/
        ├── RegisteredResources/               # Custom media assets embedded in visuals
        │   ├── dollar5533101165046277.png     # Financial / Currency icons
        │   ├── gas-pump-alt2593692500883096.png # Fuel & Gas KPI graphics
        │   └── shipping-timed3665055514870691.png # Shipping & Logistics visual cues
        └── SharedResources/
            ├── BaseThemes/                    # Theme definitions (e.g., CY26SU02.json)
            └── BuiltInThemes/                 # Power BI presets (e.g., Temperature.json)
```

---

## 🚀 Getting Started

### Prerequisites

- [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) (latest version recommended).
- Access credentials for underlying data sources (if live connection or refresh is required).

### How to Open & Edit

1. **Cloning the Repository:**
   ```bash
   git clone https://github.com/your-username/your-powerbi-repo.git
   cd your-powerbi-repo
   ```

2. **Opening in Power BI Desktop:**
   * If working with extracted Power BI Project format (`.pbip`), open the `.pbip` root file directly in Power BI Desktop.
   * If compiled as a single `.pbix` / `.pbit` file, double-click the file to open.

3. **Data Refresh:**
   * Open **Transform Data** (Power Query Editor) to inspect data source parameters.
   * Update credentials under **File > Options and Settings > Data Source Settings** if prompted.
   * Click **Refresh** on the Home tab to load the latest data into the `DataModel`.

---

## 🎨 Themes & Custom Visuals

- **Base Theme**: Custom corporate JSON palette (`CY26SU02.json`).
- **Color Temperature Theme**: Pre-configured dynamic conditional formatting theme (`Temperature.json`).
- **Custom Icons**: Custom-built icons representing key operational drivers (Currency, Fuel, Shipping speed).

---

## 🛠️ Data Model & Calculations

The data model connects operational transactions with dimension tables:
- **Fact Tables**: Logistics shipments, fuel expenditures, financial transactions.
- **Dimensions**: Date/Calendar dimension, Locations, Service levels, Asset/Vehicle IDs.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/NewVisuals`).
3. Commit changes (Ensure `.pbip` text formats are used to minimize merge conflicts if tracking raw JSON changes).
4. Push to the branch (`git push origin feature/NewVisuals`).
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.