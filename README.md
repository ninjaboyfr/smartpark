# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SmartPark - Fremtidens Cykelparkering</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>SmartPark</h1>
    <nav>
      <a href="#about">Om os</a>
      <a href="#features">Funktioner</a>
      <a href="#contact">Kontakt</a>
    </nav>
  </header>
  <main>
    <section id="intro">
      <h2>Velkommen til fremtidens cykelparkering</h2>
      <p>Med SmartPark tilbyder vi sikre, moderne og teknologisk avancerede cykelparkeringsløsninger.</p>
    </section>
    <section id="about">
      <h2>Om os</h2>
      <p>SmartPark er dedikeret til at revolutionere cykelparkering med innovation og smart teknologi.</p>
    </section>
    <section id="features">
      <h2>Funktioner</h2>
      <ul>
        <li>Smartlåger med kodelåse</li>
        <li>App-integration for reservation</li>
        <li>Bæredygtigt design</li>
      </ul>
    </section>
    <section id="contact">
      <h2>Kontakt os</h2>
      <form>
        <label for="name">Navn:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="email">Smartpark@gmail.com:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="message">Besked:</label>
        <textarea id="message" name="message" required></textarea>
        
        <button type="submit">Send</button>
      </form>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 SmartPark</p>
  </footer>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.6;
  background-color: #f9f9f9;
  color: #333;
}

header {
  background: #0047ab;
  color: #fff;
  padding: 1rem 0;
  text-align: center;
}

header nav a {
  margin: 0 15px;
  color: #fff;
  text-decoration: none;
}

main {
  padding: 1rem;
}

section {
  margin: 20px 0;
  padding: 20px;
  background: #fff;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

footer {
  text-align: center;
  padding: 1rem;
  background: #333;
  color: #fff;
}
