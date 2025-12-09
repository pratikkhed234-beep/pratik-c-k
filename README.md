<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>GrapeMart – Buy & Sell Fresh Grapes</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>🍇HEMANT TRADERS</h1>
    <p>Fresh Grapes Directly from Farmers to You!</p>
  </header>

  <section class="filters">
    <select id="locationFilter">
      <option value="all">All Locations</option>
      <option value="Bijapur">Bijapur</option>
      <option value="Godihal">Godihal</option>
      <option value="Chadchan">Chadchan</option>
      <option value="Bagalkote">Bagalkote</option>
      <option value="Gulbarga">Gulbarga</option>
    </select>

    <select id="sortPrice">
      <option value="default">Sort by Price</option>
      <option value="low-high">Low to High</option>
      <option value="high-low">High to Low</option>
    </select>
  </section>

  <section id="grapeList" class="grape-list"></section>

  <section class="order-section">
    <h2>Order Now</h2>
    <form id="orderForm">
      <label for="grapeName">Select Grape:</label>
      <select id="grapeName"></select>

      <label for="quantity">Quantity (kg):</label>
      <input type="number" id="quantity" min="1" value="1" required />
3
      <button type="submit">Place Order</button>
    </form>
    <p id="orderSummary"></p>
  </section>

  <section class="order-history">
    <h2>🧾 Order History</h2>
    <table id="orderTable">
      <thead>
        <tr>
          <th>Grape Name</th>
          <th>Quantity (kg)</th>
          <th>Price/kg (₹)</th>
          <th>Total (₹)</th>
          <th>Location</th>
          <th>Date</th>
        </tr>
      </thead>
      <tbody></tbody>
    </table>
  </section>

  <footer>
    <p>© 2025 GrapeMart | Fresh from the Vineyards of Karnataka 🍇</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
