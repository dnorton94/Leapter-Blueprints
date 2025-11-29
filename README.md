# Leapter Business Logic Projects (JavaScript)

This repository contains a **collection of business logic projects built in Leapter**, exported as **JavaScript source code**. Each project represents a **complete, executable workflow** for processing data, enforcing business rules, and producing deterministic outputs.

This repository serves as a **catalog of business logic workflows**, ready to run, review, and integrate.

---

## 📌 Overview

- **Collection of Projects:** Each folder contains a distinct business logic workflow.  
- **Executable JavaScript:** Run the code using Node.js.  
- **Deterministic & Auditable:** Predictable results for the same input data.  
- **Extensible & Reusable:** Can be integrated into larger systems or extended for new requirements.  
- **Cross-Functional Friendly:** Designed in Leapter to bridge business requirements and technical implementation.

---

## 🗂️ Repository Structure

├── projects/
│ ├── car-rental-pricing/ # Example project: Car Rental Pricing System
│ │ ├── executeLogicFlow.js
│ │ ├── inputs.json
│ │ └── README.md # Optional project-specific README
│ ├── project-2/
│ │ └── ...
│ └── ...
├── scripts/ # Optional helper scripts
├── docs/ # Documentation, diagrams, or workflow notes
└── README.md

yaml
Copy code

---

## 🚀 Getting Started

### Prerequisites

- Node.js >= 18  

### Running a Project

1. Navigate to the project folder:

```bash
cd projects/car-rental-pricing
Install dependencies if applicable:

bash
Copy code
npm install
Run the logic function:

bash
Copy code
node executeLogicFlow.js
Modify inputs.json or pass inputs programmatically.

📖 Example Project: Car Rental Pricing System
Description:
Calculates rental prices based on car model, rental duration, customer age, and fuel charges upon return. Applies surcharges for young drivers and enforces age restrictions.

Example Input (inputs.json):

json
Copy code
{
  "carModel": "Compact",
  "customerAge": 22,
  "fuelMissingLiters": 5,
  "rentalDurationDays": 3
}
Example Output:

json
Copy code
{
  "rentalPrice": 138,
  "fuelCharge": 12.5,
  "finalCost": 150.5,
  "errorMessage": null
}
Usage in JavaScript:

javascript
Copy code
const executeLogicFlow = require('./executeLogicFlow');

const input = {
  carModel: "Compact",
  customerAge: 22,
  fuelMissingLiters: 5,
  rentalDurationDays: 3
};

const result = executeLogicFlow(input);
console.log(result);
📦 Adding New Projects
Place new projects in the projects/ folder.

Include executeLogicFlow.js (or equivalent entry point) and inputs.json.

Add a short description and example inputs/outputs in a README.md inside the project folder.

Test all projects for deterministic outputs before merging.

⚖️ License
[Specify your license here, e.g., MIT, Apache 2.0]
