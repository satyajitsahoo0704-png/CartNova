# 🛒 CartNova

> **A Smart Shopping Cart and Self-Billing System for Faster, Smarter, and More Efficient Retail**

[![Smart India Hackathon](https://img.shields.io/badge/Smart%20India%20Hackathon-Prototype-orange)](https://www.sih.gov.in/)
[![Built With](https://img.shields.io/badge/Built%20With-HTML%20%7C%20CSS%20%7C%20JavaScript-blue)](#-technology-stack)
[![Status](https://img.shields.io/badge/Status-Prototype-success)](#-project-status)

## 📌 Project Overview

CartNova is a smart retail shopping cart prototype developed for the **Smart India Hackathon (SIH)**. The system combines barcode-based product scanning, real-time cart billing, inventory monitoring, low-stock alerts, and simulated digital payments in a single user-friendly interface.

The goal is to reduce checkout queues, improve shopping convenience, and help store managers monitor inventory more effectively.

## 🎯 Problem Statement

Traditional retail checkout systems can create several challenges:

- Long queues during peak shopping hours
- Manual billing and product entry
- Delays caused by centralized checkout counters
- Limited visibility into real-time inventory levels
- Difficulty identifying products that need restocking
- Increased workload for store staff

These issues affect both customer satisfaction and retail operational efficiency.

## 💡 Proposed Solution

CartNova shifts essential checkout activities from the billing counter to the shopping cart itself.

Customers can simulate scanning products while shopping, view their running bill, and proceed to a digital payment screen. At the same time, store managers can monitor product quantities, stock status, alerts, and cart connectivity from a central dashboard.

### Core Workflow

```text
Product Selection / Barcode Scan
              ↓
      Product Added to Cart
              ↓
       Live Total Calculation
              ↓
        Payment Simulation
              ↓
     Inventory Stock Deduction
              ↓
      Updated Manager Dashboard
```

## ✨ Key Features

### Customer-Facing Smart Cart

- In-cart TFT-style display simulator
- Product barcode scanning simulation
- Product quantity and price display
- Live cart total calculation
- Proceed-to-payment workflow

### Manager Dashboard

- Total product count
- Total available stock
- Low-stock product count
- Active cart status
- Inventory overview table
- Real-time inventory alerts

### Inventory Management

- Product ID and category information
- Barcode details
- Product pricing
- Current stock levels
- Automatic `OK` and `RESTOCK` status indicators
- Reorder-level monitoring

### Digital Payment Simulation

- UPI-style payment screen
- Dynamic cart amount display
- QR-style payment visual
- Simulated payment confirmation
- Automatic inventory deduction after payment

### Responsive User Interface

- Desktop, tablet, and mobile support
- Glassmorphism-inspired dashboard design
- Responsive grids and tables
- Modern visual feedback and status badges

## 🚀 Innovation and Uniqueness

CartNova combines the following capabilities in one lightweight prototype:

1. **Self-billing at the cart level** to reduce dependency on checkout counters.
2. **Real-time inventory visibility** for store managers.
3. **Hardware-ready architecture concept** designed to represent barcode scanners, ESP32 controllers, and TFT displays.
4. **Instant stock synchronization** after a completed transaction.
5. **Simple and scalable interface** that can be extended into a production-ready retail platform.

## 👥 Target Users

- Supermarkets and retail stores
- Store managers and inventory teams
- Customers seeking faster checkout
- Retail technology providers
- Smart retail and IoT solution developers

## 🌍 Expected Impact

CartNova is designed to help:

- Reduce checkout waiting time
- Improve customer shopping experience
- Reduce manual billing effort
- Improve inventory awareness
- Identify restocking requirements earlier
- Provide a foundation for IoT-enabled retail automation

## 🧰 Technology Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **UI Layout:** CSS Grid, Flexbox, responsive media queries
- **Interaction:** Browser DOM APIs and JavaScript event handlers
- **Prototype Hardware Concept:** Barcode scanner, ESP32 microcontroller, and TFT display
- **Payment Concept:** UPI dynamic QR workflow simulation

The current prototype has no external dependencies, backend service, or database.

## 📂 Project Structure

The prototype is currently implemented as a self-contained HTML application:

```text
CartNova/
├── index.html       # Application UI, CSS, product data, and JavaScript logic
└── README.md        # Project and hackathon documentation
```

If the application file has a different name in your local copy, open that HTML file in a browser.

## ▶️ Setup and Demonstration

### Run Locally

1. Clone or download this repository.
2. Open the project directory.
3. Open the HTML application file in a modern browser.

For a local development server, use Visual Studio Code Live Server or run:

```bash
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in your browser.

### Demonstrate the Prototype

1. Open the **Dashboard** and review the initial inventory statistics.
2. Navigate to **Smart Cart**.
3. Select products from the scanner simulator or click **Simulate Scan**.
4. Review the scanned products and running total.
5. Click **Proceed to Payment**.
6. Click **Simulate UPI Payment**.
7. Return to the Dashboard or Inventory page.
8. Verify that purchased quantities have been deducted from stock.

## 🧪 Project Status

**Current status: Working frontend prototype**

The present version demonstrates the complete user journey using in-memory sample data. It is intended for hackathon demonstration and proof-of-concept evaluation.

## ⚠️ Prototype Limitations

- Data is stored only in browser memory.
- Refreshing the page resets the cart and inventory.
- Barcode scanning is represented by buttons rather than a physical scanner.
- The QR code is a visual placeholder and is not a real payment QR code.
- Payment processing is simulated and does not connect to UPI providers.
- No backend API or database is connected.
- Cart items cannot currently be removed or edited manually.
- Transaction history and receipt generation are not yet implemented.

## 🔮 Future Scope

### Hardware Integration

- Connect a real barcode or QR scanner
- Integrate an ESP32 microcontroller
- Add a physical TFT display to the cart
- Capture cart telemetry and connectivity status

### Software and Platform Enhancements

- Add a backend API and persistent database
- Implement authentication and role-based access
- Add real UPI payment integration
- Support cart item removal and quantity adjustment
- Prevent quantities from exceeding available stock
- Add transaction history, invoices, and sales analytics
- Add product search, filtering, and category management
- Monitor multiple smart carts in real time
- Use WebSockets for live inventory synchronization

## 📊 Sample Product Catalog

The prototype includes ten sample retail products:

| Product | Category | Price |
| --- | --- | ---: |
| Lays Classic Salted | Snacks | ₹20 |
| Coca Cola 500ml | Beverages | ₹40 |
| Dairy Milk 40g | Chocolate | ₹50 |
| Kurkure Masala Munch | Snacks | ₹20 |
| Pepsi 500ml | Beverages | ₹40 |
| Maggi 70g | Instant Food | ₹15 |
| Britannia Good Day | Biscuits | ₹30 |
| Colgate 100g | Personal Care | ₹65 |
| Lux Soap 100g | Personal Care | ₹40 |
| Tata Salt 1kg | Grocery | ₹30 |

## 🏆 Hackathon Value Proposition

CartNova presents a practical, scalable, and hardware-compatible approach to modernizing everyday retail. By combining smart-cart interaction, self-billing, inventory intelligence, and digital payment readiness, the project addresses both customer convenience and store operations.

The prototype can serve as the foundation for a complete smart retail ecosystem suitable for supermarkets, campus stores, hospitals, airports, and other high-footfall environments.

## 👨‍💻 Team and Contribution

CartNova is developed as a Smart India Hackathon prototype. The project can be extended with team member details, institutional affiliation, problem statement ID, and presentation links for final submission.

## 📄 License

This project is provided for educational, demonstration, and Smart India Hackathon prototype purposes.
