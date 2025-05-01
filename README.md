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
      padding: 20px;
      text-align: center;
    }

    .banner {
      width: 200px;
      display: block;
      margin: 20px auto 0;
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

    .product-card h3 {
      margin: 10px 0 5px;
      font-size: 1.1em;
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
    <img class="banner" src="https://i.postimg.cc/XY83vZVN/1.png" alt="Logo Altaïr Innovations Store" />
  </header>

  <div class="socials">
    <a class="tiktok" href="https://www.tiktok.com/@altair.innovation?_t=ZN-8vzX4FCul78&_r=1" target="_blank">TikTok</a>
    <a class="instagram" href="https://www.instagram.com/kbichr?igsh=YWk5bDhkMzRpM21u" target="_blank">Instagram</a>
    <a class="youtube" href="https://www.youtube.com/@AltairInnovationStore" target="_blank">YouTube</a>
  </div>

  <section class="products">
    <div class="product-card">
      <h3>Imprimante Bluetooth sans encre</h3>
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
      <h3>Mini ventilateur portable USB</h3>
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

    <label for="product">Produit</label>
    <select name="product" id="product" required>
      <option value="">-- Choisissez un produit --</option>
      <option value="Imprimante Bluetooth">Imprimante Bluetooth sans encre</option>
      <option value="Support téléphone">Support téléphone magnétique</option>
      <option value="Briquet USB">Briquet électronique USB</option>
      <option value="Organisateur de câble">Organisateur de câble</option>
      <option value="Mini Ventilateur">Mini ventilateur portable USB</option>
    </select>

    <label for="quantity">Quantité</label>
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
