<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Diarrhea Express</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #fff4b8, #f5c77d, #b98952);
      color: #222;
      overflow-x: hidden;
    }

    header {
      background: #1f1f1f;
      color: white;
      padding: 30px;
      border-bottom: 5px solid #ffd54f;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }

    .container {
      max-width: 1200px;
      margin: auto;
      padding: 20px;
    }

    .header-flex {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 20px;
    }

    h1 {
      font-size: 4rem;
      font-weight: 900;
    }

    .tagline {
      font-size: 1.4rem;
      font-style: italic;
      color: #ffe082;
      margin-top: 10px;
    }

    .emergency-btn {
      background: #d32f2f;
      color: white;
      border: none;
      padding: 18px 28px;
      font-size: 1.1rem;
      font-weight: bold;
      border-radius: 18px;
      cursor: pointer;
      animation: pulse 1.2s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.08); }
      100% { transform: scale(1); }
    }

    .hero {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 50px;
      align-items: center;
      padding: 80px 20px;
    }

    .hero h2 {
      font-size: 4rem;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 1.5rem;
      margin-bottom: 30px;
      line-height: 1.5;
    }

    .btn-group {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }

    .btn {
      padding: 18px 26px;
      border-radius: 18px;
      border: none;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    .yellow {
      background: #ffd54f;
      color: black;
    }

    .black {
      background: #222;
      color: white;
    }

    .btn:hover {
      transform: scale(1.05);
    }

    .card {
      background: white;
      border-radius: 35px;
      padding: 40px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      transform: rotate(2deg);
      border: 4px solid #6d4c41;
      text-align: center;
    }

    .card h3 {
      font-size: 2rem;
      margin: 20px 0;
    }

    .card ul {
      list-style: none;
      font-size: 1.2rem;
      line-height: 2;
      font-weight: bold;
    }

    .section {
      padding: 80px 20px;
    }

    .section-title {
      text-align: center;
      font-size: 3.5rem;
      margin-bottom: 50px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .service-box,
    .testimonial {
      background: rgba(255,255,255,0.9);
      border-radius: 30px;
      padding: 30px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      transition: 0.3s;
    }

    .service-box:hover,
    .testimonial:hover {
      transform: translateY(-5px);
    }

    .service-box h3 {
      font-size: 1.8rem;
      margin-bottom: 15px;
    }

    .emoji {
      font-size: 4rem;
      margin-bottom: 20px;
    }

    .stats {
      background: black;
      color: white;
      padding: 70px 20px;
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 30px;
      text-align: center;
    }

    .stat-number {
      font-size: 4rem;
      font-weight: 900;
      color: #ffd54f;
    }

    footer {
      text-align: center;
      padding: 50px 20px;
      font-size: 1.2rem;
      font-weight: bold;
    }

    .fake-alert {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #d32f2f;
      color: white;
      padding: 18px 24px;
      border-radius: 18px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      font-weight: bold;
      animation: pulse 1.5s infinite;
    }
  </style>
</head>
<body>

  <header>
    <div class="container header-flex">
      <div>
        <h1>💩 Diarrhea Express</h1>
        <div class="tagline">“Here to service your diarrhea needs.”</div>
      </div>

      <button class="emergency-btn" onclick="activateEmergency()">
        EMERGENCY DELIVERY
      </button>
    </div>
  </header>

  <section class="hero container">
    <div>
      <h2>Fast. Violent. Reliable.</h2>

      <p>
        Whether it’s taco night gone wrong or a suspicious gas station burrito,
        Diarrhea Express is standing by with elite-level emergency response.
      </p>

      <div class="btn-group">
        <button class="btn yellow">Schedule an Incident</button>
        <button class="btn black">Track Your Plumber</button>
      </div>
    </div>

    <div class="card">
      <div style="font-size: 7rem;">🚽</div>
      <h3>24/7 Emergency Response</h3>

      <ul>
        <li>✅ Toilet Tactical Teams</li>
        <li>✅ Brown Alert Monitoring</li>
        <li>✅ Splash Containment Units</li>
        <li>✅ Family Pack Discounts</li>
      </ul>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <h2 class="section-title">Premium Services</h2>

      <div class="grid">
        <div class="service-box">
          <div class="emoji">🚚</div>
          <h3>Code Brown Priority Shipping</h3>
          <p>
            Our drivers arrive before you finish regretting the sushi.
          </p>
        </div>

        <div class="service-box">
          <div class="emoji">🧻</div>
          <h3>Industrial Strength Support</h3>
          <p>
            For festivals, weddings, and chili cookoffs gone catastrophically wrong.
          </p>
        </div>

        <div class="service-box">
          <div class="emoji">💨</div>
          <h3>Express Flush Membership</h3>
          <p>
            Unlimited emergency visits and complimentary air fresheners.
          </p>
        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <h2 class="section-title">Customer Testimonials</h2>

      <div class="grid">
        <div class="testimonial">
          <p>
            “I trusted a gas station egg salad sandwich. Diarrhea Express saved my marriage.”
          </p>
          <br>
          <strong>— Gary from Ohio</strong>
        </div>

        <div class="testimonial">
          <p>
            “Five stars. The technician arrived wearing a hazmat suit and carrying wet wipes.”
          </p>
          <br>
          <strong>— Melissa P.</strong>
        </div>

        <div class="testimonial">
          <p>
            “I clicked the emergency button and heard sirens almost immediately.”
          </p>
          <br>
          <strong>— Anonymous</strong>
        </div>
      </div>
    </div>
  </section>

  <section class="stats">
    <div class="container stats-grid">
      <div>
        <div class="stat-number">14,223</div>
        <div>Emergency Flushes</div>
      </div>

      <div>
        <div class="stat-number">97%</div>
        <div>Panic Reduction</div>
      </div>

      <div>
        <div class="stat-number">3 mins</div>
        <div>Average Arrival Time</div>
      </div>

      <div>
        <div class="stat-number">∞</div>
        <div>Regrets Prevented</div>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2026 Diarrhea Express LLC</p>
    <p style="margin-top: 10px; font-style: italic;">
      Proudly serving stomach disasters nationwide.
    </p>
  </footer>

  <div class="fake-alert" id="alertBox">
    🚨 ACTIVE CODE BROWN IN YOUR AREA 🚨
  </div>

  <script>
    function activateEmergency() {
      alert('🚨 EMERGENCY RESPONSE TEAM DISPATCHED 🚽\n\nEstimated arrival time: 2 minutes.');
    }

    setTimeout(() => {
      const alertBox = document.getElementById('alertBox');
      alertBox.style.display = 'none';
    }, 8000);
  </script>

</body>
</html>
