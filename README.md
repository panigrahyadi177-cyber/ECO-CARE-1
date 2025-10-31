<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ECO CARE</title>
<style>
  body {
    font-family: "Poppins", sans-serif;
    background: linear-gradient(135deg, #00c16e, #00a8cc);
    color: #fff;
    text-align: center;
    margin: 0;
    padding: 0;
  }
  header {
    padding: 20px;
    background: rgba(0,0,0,0.3);
  }
  h1 { margin: 0; font-size: 28px; }
  section {
    margin: 20px;
    background: rgba(255,255,255,0.2);
    border-radius: 15px;
    padding: 20px;
  }
  button {
    background: #004d00;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 10px;
    font-size: 16px;
  }
  .fact-box {
    margin-top: 10px;
    font-style: italic;
    background: rgba(255,255,255,0.3);
    border-radius: 10px;
    padding: 10px;
  }
</style>
</head>
<body>
<header>
  <h1> ECO CARE</h1>
  <p>Learn how to protect our planet through recycling and sustainable living!</p>
</header>

<section>
  <h2>Did You Know?</h2>
  <button onclick="showFact()">Show Eco Fact</button>
  <div id="fact" class="fact-box"></div>
</section>

<section>
  <h2>Green Living Tips </h2>
  <ul style="text-align:left; max-width:400px; margin:auto;">
    <li>Use reusable bottles and bags.</li>
    <li>Segregate waste into dry and wet bins.</li>
    <li>Recycle plastic, metal, and glass materials.</li>
    <li>Turn off lights when not in use.</li>
    <li>Plant trees and support local green drives.</li>
  </ul>
</section>

<footer>
  <p>Made with  by Aditya Kumar</p>
</footer>

<script>
const facts = [
  "Recycling one aluminum can saves enough energy to run a TV for 3 hours!",
  "Plastic takes up to 500 years to decompose — recycle it responsibly.",
  "Every ton of recycled paper saves 17 trees!",
  "LED bulbs reduce carbon emissions by 80%.",
  "Composting kitchen waste reduces landfill load by 30%."
];
function showFact() {
  document.getElementById("fact").textContent =
    facts[Math.floor(Math.random()*facts.length)];
}
</script>
</body>
</html>
