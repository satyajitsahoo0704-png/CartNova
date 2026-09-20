# CartNova

CartNova is a browser-based smart shopping cart and inventory monitoring prototype created for the Smart India Hackathon (SIH). It demonstrates how a connected shopping cart could support barcode-based product scanning, self-billing, inventory tracking, low-stock alerts, and digital payment simulation.

## Features

- Manager dashboard with real-time inventory statistics
- Smart cart interface styled as an in-cart TFT display
- Simulated barcode scanning
- Product catalog with categories, barcodes, prices, and stock levels
- Automatic cart quantity and total calculations
- Inventory status indicators and low-stock alerts
- Simulated UPI payment flow
- Automatic stock deduction after a successful payment
- Responsive layout for desktop, tablet, and mobile screens
- Glassmorphism-inspired user interface

## Application Sections

### Dashboard

The dashboard displays:

- Total number of products
- Total available stock
- Number of low-stock products
- Active cart status
- Inventory overview
- Inventory alerts

### Smart Cart

The Smart Cart page simulates the display mounted on a physical shopping cart. Users can select products from the scanner simulator or use the **Simulate Scan** button to add a randomly selected product to the cart.

The cart displays:

- Scanned products
- Quantities
- Individual item totals
- Current cart total
- Proceed-to-payment action

### Inventory

The Inventory page shows the complete product catalog, including:

- Product ID
- Product name
- Category
- Barcode
- Price
- Current stock
- Stock status

### Payment

The Payment page provides a demonstration UPI payment screen with a QR-style visual, payable amount, and **Simulate UPI Payment** button.

> This is a prototype. The QR graphic and payment action do not connect to a real UPI provider or financial service.

## Technology Stack

- HTML5
- CSS3
- Vanilla JavaScript
- CSS Grid and Flexbox
- Responsive media queries
- Browser DOM APIs

The project has no external dependencies, build tools, or backend services.

## Project Structure

The application is currently implemented as a single self-contained HTML file:

```text
CartNova/
└── index.html    # HTML structure, CSS styles, product data, and application logic
```

If the HTML file has a different name in your local copy, open that file in a browser.

## Running the Project

### Option 1: Open directly in a browser

1. Clone or download this repository.
2. Open the HTML application file in a modern browser.

### Option 2: Use a local development server

With Visual Studio Code:

1. Install the **Live Server** extension.
2. Open the repository folder.
3. Right-click the HTML file.
4. Select **Open with Live Server**.

Alternatively, with Python installed, run the following from the project directory:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000) in your browser.

## How to Use

1. Open the **Dashboard** to review inventory statistics.
2. Open **Smart Cart** to add products using the product buttons.
3. Use **Simulate Scan** to add a random product.
4. Review the cart contents and total.
5. Select **Proceed to Payment**.
6. Select **Simulate UPI Payment** to complete the demonstration transaction.
7. Return to the Dashboard or Inventory page to see the updated stock levels.

## Sample Product Catalog

The prototype includes ten sample products:

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

Product data is stored in the JavaScript `products` array and can be edited directly in the HTML file.

## Main JavaScript Functions

| Function | Purpose |
| --- | --- |
| `showPage(page)` | Switches between Dashboard, Smart Cart, Inventory, and Payment views |
| `updateInventory()` | Rebuilds inventory tables and dashboard statistics |
| `updateAlerts()` | Displays products below their reorder level |
| `createProductButtons()` | Generates the product scanner controls |
| `addToCart(productID)` | Adds a product or increases its cart quantity |
| `updateCart()` | Refreshes cart items, totals, and payment amount |
| `simulateScan()` | Adds a randomly selected product to the cart |
| `paymentSuccess()` | Simulates payment and deducts purchased quantities from stock |

## Current Limitations

- Data is stored only in browser memory.
- Refreshing the page resets the cart and inventory.
- Barcode scanning is simulated with buttons rather than a physical scanner.
- The QR code is a visual placeholder and is not a real payment QR code.
- No backend API or database is connected.
- Payment processing is not real.
- Cart quantities cannot currently be removed or edited manually.
- The prototype does not persist transaction history.

## Future Improvements

- Connect the interface to a backend API and database
- Integrate a real barcode or QR scanner
- Connect the system to an ESP32 or other IoT controller
- Add authentication and manager/customer roles
- Add real UPI payment integration
- Add cart item removal and quantity controls
- Prevent cart quantities from exceeding available stock
- Add transaction history, receipts, and sales reports
- Add product search, filtering, and category management
- Support monitoring multiple smart carts in real time
- Use WebSockets for live inventory and cart telemetry

## Browser Support

CartNova is designed for modern browsers that support HTML5, CSS Grid, Flexbox, JavaScript template literals, and standard DOM APIs.

Recommended browsers:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

## License

This project is provided for educational, demonstration, and Smart India Hackathon prototype purposes.
