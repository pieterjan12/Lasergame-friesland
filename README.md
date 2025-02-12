
<html lang="nl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lasergame Verhuur</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      color: #333;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #333;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      text-align: center;
      margin: 20px 0;
    }
    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #333;
      font-weight: bold;
    }
    section {
      padding: 20px;
      margin: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    form input, form select, form button {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      background-color: #007BFF;
      color: white;
      border: none;
      cursor: pointer;
    }
    form button:hover {
      background-color: #0056b3;
    }
  </style>
  <script>
    function updatePrice() {
      const quantity = document.getElementById("quantity").value;
      const price = quantity * 5; // €5 per lasergame
      document.getElementById("totalPrice").value = "€" + price;
    }
  </script>
</head>
<body>

<header>
  <h1>Lasergame Verhuur friesland</h1>
  <p>De beste lasergames huren voor elk evenement!</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#about">Over Ons</a>
  <a href="#pricing">Prijzen</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <h2>Welkom bij Lasergame friesland Verhuur</h2>
  <p>Wij bieden hoogwaardige lasergames aan voor elk feest of evenement. Ideaal voor verjaardagen, bedrijfsuitjes en meer!</p>
</section>

<section id="about">
  <h2>Over Ons</h2>
  <p>wij verhuren lasergame. wij voorzien u van lasergame-apparatuur. Ons doel is om jouw evenement onvergetelijk te maken!</p>
</section>

<section id="pricing">
  <h2>Prijzen</h2>
  <p>De huurprijs is €5 per lasergame. Kies het gewenste aantal (maximaal 12 stuks).</p>
</section>

<section id="contact">
  <h2>Contact</h2>
  <form action="mailto:pieterjanwijnsma79@gmail.com" method="POST" enctype="text/plain">
    <label for="quantity">Hoeveel lasergames wil je huren?</label>
    <select id="quantity" name="Aantal Lasergames" onchange="updatePrice()" required>
      <option value="1">1 lasergame (€5)</option>
      <option value="2">2 lasergames (€10)</option>
      <option value="3">3 lasergames (€15)</option>
      <option value="4">4 lasergames (€20)</option>
      <option value="5">5 lasergames (€25)</option>
      <option value="6">6 lasergames (€30)</option>
      <option value="7">7 lasergames (€35)</option>
      <option value="8">8 lasergames (€40)</option>
      <option value="9">9 lasergames (€45)</option>
      <option value="10">10 lasergames (€50)</option>
      <option value="11">11 lasergames (€55)</option>
      <option value="12">12 lasergames (€60)</option>
    </select>

    <label for="totalPrice">Totaalbedrag:</label>
    <input type="text" id="totalPrice" name="Totaalbedrag" readonly>

    <label for="date">Datum van afhalen:</label>
    <input type="date" id="date" name="Afhaaldatum" required>

    <label for="time">Tijd van afhalen:</label>
    <input type="time" id="time" name="Afhaaltijd" required>

    <label for="email">Je e-mailadres:</label>
    <input type="email" id="email" name="E-mailadres" placeholder="Vul je e-mailadres in" required>

    <button type="submit">Verzenden</button>
  </form>
</section>

<footer>
  <p>&copy; 2025 Lasergame Verhuur. Alle rechten voorbehouden.</p>
</footer>

