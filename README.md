<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Keen Media House</title>
  <link rel="stylesheet" href="styles.css" />
  <style>
    h2 {
      color: #2b5dff;
    }
    ul li strong {
      color: #4caf50;
    }
    #services ul li {
      color: #000;
      font-weight: bold;
    }
    .gallery-image {
      width: 200px;
      height: auto;
      margin: 10px;
      border: 2px solid #ddd;
      border-radius: 8px;
    }
    #flyer-sample {
      margin: 20px auto;
      display: block;
      width: 90%;
      max-width: 600px;
      border: 3px solid #000;
      border-radius: 10px;
    }
    #services ul li span {
      color: #000;
    }
    .contact-info {
      margin-top: 30px;
      padding: 15px;
      background-color: #f1f1f1;
      border-top: 2px solid #4caf50;
      text-align: center;
    }
    .contact-info h3 {
      color: #2b5dff;
    }
    .contact-info p, .contact-info a {
      color: #000;
      margin: 5px 0;
      display: block;
    }
    .contact-info a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <header>
    <h1 style="color: #4caf50;">Keen Media House</h1>
    <p style="color: #ff9800;">Capturing Moments, Creating Memories</p>
  </header>

  <section id="about">
    <h2>About Us</h2>
    <p>Welcome to Keen Media House, proudly located in the vibrant town of Eldoret, Kenya. Since our inception in 2019, we have become a trusted name in photography and videography. We specialize in crafting powerful visual stories that preserve your most cherished memories with creativity, clarity, and class.</p>
    <p>Our studio was founded on a passion for excellence, artistry, and a desire to serve our clients with the utmost professionalism. All our team members bring a minimum of five years of experience in the field, ensuring that every shot we take and every video we produce meets the highest standards.</p>
    <p>At Keen Media House, we invest in state-of-the-art equipment and cutting-edge editing tools to deliver stunning results. From modern DSLR and mirrorless cameras, drones for aerial cinematography, to advanced lighting and studio setups—our gear empowers us to work magic through the lens. Our post-production is fueled by industry-standard software, delivering breathtaking visuals that go beyond expectations.</p>
    <p>Whether it's a wedding, a corporate shoot, a personal portrait, or a commercial campaign, our mission is to transform moments into masterpieces. Our commitment to quality, attention to detail, and artistic flair is what makes us stand out in the competitive media landscape.</p>
    <p>We are dedicated to professionalism and transparency. For all bookings, a 15% deposit is required prior to the day of work to secure your session. The remaining balance is to be settled immediately before our team leaves the site. This policy ensures smooth planning, mutual commitment, and an exceptional experience for every client.</p>
    <p>Thank you for choosing Keen Media House—where every frame tells a story worth remembering.</p>
    <ul>
      <li><strong>Photographers:</strong> Billino Kerich & Meshack Collins Kipchirchir</li>
      <li><strong>Videographers:</strong> John Olwoch & Mercy Wanjiku</li>
      <li><strong>Drone Operator:</strong> Julia Maina</li>
    </ul>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <ul>
      <li><span>Food Photography</span> - <strong>KES 3,000</strong></li>
      <li><span>Event Photography</span> - <strong>KES 10,000</strong></li>
      <li><span>Wedding Photography</span> - <strong>KES 25,000</strong></li>
      <li><span>Portrait Photography</span> - <strong>KES 5,000</strong></li>
      <li><span>Headshot Photography</span> - <strong>KES 4,000</strong></li>
      <li><span>Commercial Photography</span> - <strong>KES 15,000</strong></li>
      <li><span>Real Estate Photography</span> - <strong>KES 8,000</strong></li>
    </ul>
  </section>

  <section id="gallery">
    <h2>Gallery</h2>
    <div id="image-gallery">
      <img src="images/DSC_8810.jpg" alt="Sample 1" class="gallery-image">
      <img src="images/IMG-20250226-WA0007.jpg" alt="Sample 2" class="gallery-image">
      <img src="images/DSC_4113 (1).jpg" alt="Sample 3" class="gallery-image">
      <img src="images/DSC_3840.jpg" alt="Sample 4" class="gallery-image">
      <img src="images/DSC_0629.jpg" alt="Sample 5" class="gallery-image">
      <img src="images/DSC_0559.jpg" alt="Sample 6" class="gallery-image">
      <img src="images/DSC_0068.jpg" alt="Sample 7" class="gallery-image">
      <img src="images/DSC_0033 (1).jpg" alt="Sample 8" class="gallery-image">
      <img src="images/DSC_8504.jpg" alt="Sample 9" class="gallery-image">
    </div>
    <h3>Service Flyer</h3>
    <img id="flyer-sample" src="images/Keen-media-house_page-0001.jpg" alt="Keen Media House Flyer">
  </section>

  <section id="booking">
    <h2>Book a Service</h2>
    <form id="bookingForm" action="https://formspree.io/f/moqgdodg" method="POST">
      <label for="name">Full Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="service">Service:</label>
      <select id="service" name="service" required>
        <option value="">Select a Service</option>
        <option value="Food Photography">Food Photography</option>
        <option value="Event Photography">Event Photography</option>
        <option value="Wedding Photography">Wedding Photography</option>
        <option value="Portrait Photography">Portrait Photography</option>
        <option value="Headshot Photography">Headshot Photography</option>
        <option value="Commercial Photography">Commercial Photography</option>
        <option value="Real Estate Photography">Real Estate Photography</option>
      </select>

      <label for="date">Preferred Date:</label>
      <input type="date" id="date" name="date" required>

      <label for="location">Location:</label>
      <input type="text" id="location" name="location" required>

      <button type="submit">Submit Booking</button>
    </form>
    <p id="booking-status"></p>
  </section>

  <section id="admin">
    <h2>Admin Panel</h2>
    <div id="admin-login">
      <label for="admin-password">Enter Admin Password:</label>
      <input type="password" id="admin-password">
      <button onclick="loginAdmin()">Login</button>
    </div>
    <div id="admin-panel" style="display:none;">
      <h3>Booked Dates</h3>
      <ul id="bookings-list"></ul>
    </div>
  </section>

  <section class="contact-info">
    <h3>Contact Us</h3>
    <p>Phone: <a href="tel:+254707431433">+254707431433</a> / <a href="tel:+254741946669">+254741946669</a></p>
    <p>WhatsApp: <a href="https://wa.me/254707431433" target="_blank">Chat with us</a></p>
    <p>Find us on social media:</p>
    <a href="https://www.facebook.com/keenmediahouse" target="_blank">Facebook</a>
    <a href="https://www.tiktok.com/@keenmediahouse" target="_blank">TikTok</a>
    <a href="https://www.youtube.com/@keenmediahouse" target="_blank">YouTube</a>
    <a href="https://www.instagram.com/keenmediahouse" target="_blank">Instagram</a>
  </section>

  <footer>
    <p>&copy; 2025 Keen Media House. <span style="color:#ff5722;">Capturing Moments, Creating Memories.</span></p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
# keenmediahouse
