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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Upload et billede</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 20px;
      background-color: #f4f4f9;
      color: #333;
    }
    input[type="file"] {
      margin: 20px 0;
    }
    img {
      max-width: 100%;
      max-height: 300px;
      margin-top: 20px;
      border: 2px solid #ddd;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <h1>Upload og vis et billede</h1>
  <p>Vælg et billede nedenfor, og det vil blive vist her på siden.</p>
  <input type="file" id="imageInput" accept="image/*">
  <div>
    <img id="preview" alt="Billedet vil blive vist her" style="display:none;">
  </div>

  <script>
    // Hent input- og billed-elementerne
    const imageInput = document.getElementById('imageInput');
    const preview = document.getElementById('preview');

    // Tilføj en eventlistener for at opdage ændringer
    imageInput.addEventListener('change', (event) => {
      const file = event.target.files[0]; // Få det valgte filobjekt
      if (file) {
        const reader = new FileReader(); // Lav en fil-læser

        // Når filen er læst, vis billedet
        reader.onload = (e) => {
          preview.src = e.target.result; // Sæt billedets kilde til filens data
          preview.style.display = 'block'; // Vis billedet
        };

        reader.readAsDataURL(file); // Læs filen som en data-URL
      } else {
        preview.style.display = 'none'; // Skjul billedet, hvis ingen fil er valgt
      }
    });
  </script>
</body>
</html>
