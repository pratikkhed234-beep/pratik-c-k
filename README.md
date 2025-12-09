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


  /* Background Image */
body {
  margin: 0;
  font-family: "Poppins", sans-serif;
  background: url("bg1.jpg") no-repeat center center fixed;
  background-size: cover;
  color: #fff;
}

/* Soft Dark Overlay */
.bg-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.45);
  backdrop-filter: blur(3px);
  z-index: -1;
}

/* ===== HEADER ===== */
header {
  text-align: center;
  padding: 40px 20px;
}

header h1 {
  font-size: 55px;
  font-weight: 700;
  text-shadow: 0 0 25px rgba(0,0,0,0.8);
}

header p {
  font-size: 20px;
  opacity: 0.9;
}

/* ===== FILTERS ===== */
.filters {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 20px auto;
}

select {
  padding: 12px 20px;
  font-size: 17px;
  border-radius: 12px;
  border: none;
  backdrop-filter: blur(6px);
  background: rgba(255,255,255,0.35);
  color: #000;
  font-weight: 600;
  cursor: pointer;
  transition: 0.3s;
}

select:hover {
  background: rgba(255,255,255,0.6);
}

/* ===== GRAPE LIST ===== */
.grape-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
  padding: 20px;
}

/* Grape Card */
.card {
  width: 260px;
  padding: 20px;
  border-radius: 20px;
  background: rgba(255,255,255,0.20);
  backdrop-filter: blur(12px);
  color: #fff;
  text-align: center;
  box-shadow: 0 0 20px rgba(0,0,0,0.2);
  transition: transform 0.2s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

.card h3 {
  font-size: 22px;
  margin-bottom: 8px;
}

/* ===== ORDER & HISTORY BOXES ===== */
.order-section, 
.order-history {
  background: rgba(255,255,255,0.18);
  backdrop-filter: blur(12px);
  padding: 30px;
  margin: 30px auto;
  width: 90%;
  max-width: 900px;
  border-radius: 18px;
  color: #fff;
  box-shadow: 0 0 25px rgba(0,0,0,0.3);
}

.order-section h2,
.order-history h2 {
  font-size: 28px;
  margin-bottom: 10px;
}

label {
  display: block;
  margin-top: 15px;
  font-weight: 600;
}

input, select {
  width: 100%;
  padding: 12px;
  border-radius: 12px;
  border: none;
  margin-top: 5px;
}

/* ==== BUTTON ==== */
button {
  margin-top: 15px;
  padding: 12px 22px;
  background: linear-gradient(45deg, #9b00ff, #e600ff);
  color: white;
  border: none;

</body>
</html>
