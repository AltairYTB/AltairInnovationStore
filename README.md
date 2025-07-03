<DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Altaïr Innovations Store</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #0a0a0a;
      color: #ffffff;
    }

    header {
      background-color: #0a0a0a;
      padding: 10px 20px;
      display: flex;
      align-items: center;
      justify-content: flex-start;
    }

    .logo {
      width: 80px;
      cursor: pointer;
    }

    .socials {
      display: flex;
      justify-content: center;
      gap: 15px;
      margin: 30px 0;
    }

    .socials a {
      text-decoration: none;
      padding: 10px 20px;
      border-radius: 10px;
      color: #fff;
      font-weight: bold;
      transition: 0.3s;
    }

    .tiktok {
      background-color: #000;
      border: 2px solid #ff0050;
    }

    .tiktok:hover {
      background-color: #ff0050;
    }

    .youtube {
      background-color: #ff0000;
    }

    .youtube:hover {
      background-color: #cc0000;
    }

    .instagram {
      background: linear-gradient(45deg, #feda75, #fa7e1e, #d62976, #962fbf, #4f5bd5);
    }

    .instagram:hover {
      opacity: 0.8;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px;
    }

    .product-card {
      background-color: #111;
      padding: 15px;
      border-radius: 12px;
      text-align: center;
    }

    .product-card h3 a {
      color: #fff;
      text-decoration: none;
      padding: 8px 16px;
      background-color: #ff0050;
      border-radius: 8px;
      display: inline-block;
      margin-bottom: 8px;
    }

    .product-card h3 a:hover {
      background-color: #e60045;
    }

    .product-card p {
      margin: 0;
      color: #aaa;
    }

    form {
      max-width: 600px;
      margin: 0 auto 60px;
      background-color: #111;
      padding: 30px;
      border-radius: 12px;
    }

    form h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input, select, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 8px;
      border: none;
      background-color: #333;
      color: #fff;
    }

    textarea {
      resize: vertical;
    }

    .checkboxes label {
      display: flex;
      align-items: center;
      margin-top: 10px;
      font-weight: normal;
    }

    .checkboxes input {
      width: auto;
      margin-right: 10px;
    }

    button {
      margin-top: 20px;
      padding: 12px 25px;
      background-color: #ff0050;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1em;
      cursor: pointer;
      width: 100%;
    }

    button:hover {
      background-color: #e60045;
    }

    footer {
      text-align: center;
      padding: 20px;
      color: #777;
      background-color: #0a0a0a;
    }
  </style>
</head>
<body>

  <header>
    <a href="https://altairytb.github.io/AltairInnovationStore/">
      <img class="logo" src="https://i.postimg.cc/XY83vZVN/1.png" alt="Accueil" />
    </a>
  </header>

  <div class="socials">
    <a class="tiktok" href="https://www.tiktok.com/@altair.innovation?_t=ZN-8vzX4FCul78&_r=1" target="_blank">TikTok</a>
    <a class="instagram" href="https://www.instagram.com/kbichr?igsh=YWk5bDhkMzRpM21u" target="_blank">Instagram</a>
    <a class="youtube" href="https://www.youtube.com/@AltairInnovationStore" target="_blank">YouTube</a>
  </div>

  <section class="products" id="top">
    <div class="product-card">
      <h3><a href="https://altairytb.github.io/Imprimante-bluetooth/">Imprimante Bluetooth sans encre</a></h3>
      <p>29.99€</p>
    </div>
    <div class="product-card">
      <h3>Support téléphone magnétique</h3>
      <p>14.99€</p>
    </div>
    <div class="product-card">
      <h3>Briquet électronique rechargeable USB</h3>
      <p>14.99€</p>
    </div>
    <div class="product-card">
      <h3>Organisateur de câble</h3>
      <p>9.99€</p>
    </div>
    <div class="product-card">
      <h3>refroidisseur pour telephone</h3>
      <p>19.99€</p>
    </div>
  </section>

  <form action="https://formspree.io/f/meogebbb" method="POST">
    <h2>Commander un produit</h2>
    <label for="name">Nom complet</label>
    <input type="text" name="name" id="name" required>

    <label for="email">Adresse email</label>
    <input type="email" name="email" id="email" required>

    <label for="phone">Numéro de téléphone</label>
    <input type="tel" name="phone" id="phone" required>

    <label for="address">Adresse de livraison</label>
    <textarea name="address" id="address" rows="3" required></textarea>

    <label>Produits à commander</label>
    <div class="checkboxes">
      <label><input type="checkbox" name="products" value="Imprimante Bluetooth"> Imprimante Bluetooth sans encre (29.99€)</label>
      <label><input type="checkbox" name="products" value="Support téléphone"> Support téléphone magnétique (14.99€)</label>
      <label><input type="checkbox" name="products" value="Briquet USB"> Briquet USB rechargeable (14.99€)</label>
      <label><input type="checkbox" name="products" value="Organisateur câble"> Organisateur de câble (9.99€)</label>
      <label><input type="checkbox" name="products" value="Mini ventilateur"> Mini ventilateur portable (19.99€)</label>
    </div>

    <label for="quantity">Quantité totale</label>
    <input type="number" name="quantity" id="quantity" min="1" required>

    <label for="payment">Moyen de paiement</label>
    <select name="payment" id="payment" required>
      <option value="">-- Sélectionner un moyen de paiement --</option>
      <option value="Carte bancaire">Carte bancaire</option>
      <option value="PayPal">PayPal</option>
      <option value="Virement bancaire">Virement bancaire</option>
    </select>

    <label for="message">Message complémentaire</label>
    <textarea name="message" id="message" rows="3"></textarea>

    <button type="submit">Envoyer la commande</button>
  </form>

  <footer>
    &copy; 2025 Altaïr Innovations Store - Tous droits réservés
  </footer>

</body>
</html>
