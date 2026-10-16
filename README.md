<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>KS Online Services | Online Support</title>

  <meta name="description"
    content="KS Online Services provides convenient online assistance and digital support. Contact us to discuss your requirements.">

  <style>
    :root {
      --orange: #ea580c;
      --orange-light: #fff7ed;
      --dark: #292524;
      --muted: #78716c;
      --white: #ffffff;
      --border: #f0e7df;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      color: var(--dark);
      background: var(--white);
      line-height: 1.7;
    }

    a {
      text-decoration: none;
    }

    .container {
      width: min(1100px, 90%);
      margin: auto;
    }

    header {
      background: white;
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .navbar {
      min-height: 82px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
    }

    .logo {
      font-size: 23px;
      font-weight: 800;
      color: var(--dark);
    }

    .logo span {
      color: var(--orange);
    }

    nav {
      display: flex;
      align-items: center;
      gap: 25px;
    }

    nav a {
      color: var(--dark);
      font-size: 14px;
      font-weight: 600;
    }

    nav a:hover {
      color: var(--orange);
    }

    .button {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      gap: 8px;
      padding: 13px 22px;
      border-radius: 9px;
      font-weight: 700;
      border: 2px solid transparent;
      transition: 0.2s;
    }

    .button-primary {
      color: white;
      background: var(--orange);
    }

    .button-primary:hover {
      background: #c2410c;
      transform: translateY(-2px);
    }

    .button-outline {
      border-color: var(--orange);
      color: var(--orange);
      background: white;
    }

    .hero {
      padding: 100px 0;
      background:
        radial-gradient(
          circle at 90% 10%,
          #fed7aa 0,
          transparent 30%
        ),
        var(--orange-light);
    }

    .hero-content {
      max-width: 760px;
    }

    .eyebrow {
      display: inline-block;
      padding: 7px 13px;
      border-radius: 30px;
      background: #ffedd5;
      color: #9a3412;
      font-size: 13px;
      font-weight: 700;
      margin-bottom: 20px;
    }

    h1 {
      font-size: clamp(38px, 6vw, 64px);
      line-height: 1.12;
      letter-spacing: -1.5px;
      margin-bottom: 22px;
    }

    h1 span {
      color: var(--orange);
    }

    .hero p {
      color: #57534e;
      font-size: 18px;
      max-width: 600px;
      margin-bottom: 30px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    section {
      padding: 80px 0;
    }

    .section-heading {
      text-align: center;
      max-width: 650px;
      margin: 0 auto 42px;
    }

    .section-heading h2 {
      font-size: clamp(28px, 4vw, 40px);
      margin-bottom: 12px;
    }

    .section-heading p {
      color: var(--muted);
    }

    .services-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 22px;
    }

    .service-card {
      padding: 30px;
      border: 1px solid var(--border);
      border-radius: 16px;
      background: white;
      transition: 0.2s;
    }

    .service-card:hover {
      border-color: #fdba74;
      transform: translateY(-4px);
      box-shadow: 0 12px 30px #2925240d;
    }

    .service-icon {
      display: grid;
      place-items: center;
      width: 52px;
      height: 52px;
      background: var(--orange-light);
      border-radius: 13px;
      font-size: 25px;
      margin-bottom: 18px;
    }

    .service-card h3 {
      font-size: 20px;
      margin-bottom: 8px;
    }

    .service-card p {
      color: var(--muted);
      font-size: 15px;
    }

    .about {
      background: #fafaf9;
    }

    .about-content {
      max-width: 750px;
      margin: auto;
      text-align: center;
    }

    .about-content h2 {
      font-size: 36px;
      margin-bottom: 18px;
    }

    .about-content p {
      color: var(--muted);
    }

    .contact {
      background: var(--orange-light);
    }

    .contact-card {
      max-width: 760px;
      margin: auto;
      padding: 45px 30px;
      border-radius: 20px;
      background: white;
      text-align: center;
      box-shadow: 0 12px 35px #2925240b;
    }

    .contact-card h2 {
      font-size: clamp(28px, 4vw, 38px);
      margin-bottom: 12px;
    }

    .contact-card > p {
      color: var(--muted);
      margin-bottom: 25px;
    }

    .contact-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
    }

    .contact-email {
      display: block;
      margin-top: 22px;
      color: var(--dark);
      overflow-wrap: anywhere;
    }

    footer {
      padding: 28px 0;
      background: var(--dark);
      color: #e7e5e4;
      text-align: center;
      font-size: 14px;
    }

    footer p + p {
      margin-top: 5px;
      color: #a8a29e;
    }

    @media (max-width: 650px) {
      .navbar {
        padding: 15px 0;
        flex-direction: column;
      }

      nav {
        justify-content: center;
        flex-wrap: wrap;
        gap: 15px;
      }

      .hero {
        padding: 70px 0;
      }

      .services-grid {
        grid-template-columns: 1fr;
      }

      section {
        padding: 60px 0;
      }

      .service-card {
        padding: 24px;
      }

      .contact-card {
        padding: 35px 20px;
      }

      .hero-actions .button {
        width: 100%;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="container navbar">
      <a class="logo" href="#home">
        KS <span>Online Services</span>
      </a>

      <nav aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#services">Services</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container hero-content">
        <span class="eyebrow">
          Simple. Helpful. Online.
        </span>

        <h1>
          Your Online Needs,<br>
          <span>Made Easier.</span>
        </h1>

        <p>
          Welcome to KS Online Services. We aim to make
          online tasks simpler with convenient support
          tailored to your requirements.
        </p>

        <div class="hero-actions">
          <a
            class="button button-primary"
            href="https://wa.me/919927170739"
            target="_blank"
            rel="noopener noreferrer">
            Chat on WhatsApp →
          </a>

          <a class="button button-outline" href="#services">
            Explore Services
          </a>
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <div class="section-heading">
          <h2>How We Can Help</h2>
          <p>
            Explore our online service offerings and contact
            us to discuss the help you need.
          </p>
        </div>

        <div class="services-grid">
          <article class="service-card">
            <div class="service-icon">💻</div>
            <h3>Online Assistance</h3>
            <p>
              Get guidance with online tasks and learn
              about solutions suited to your needs.
            </p>
          </article>

          <article class="service-card">
            <div class="service-icon">🤝</div>
            <h3>Customer Support</h3>
            <p>
              Contact us with your questions and discuss
              the support you are looking for.
            </p>
          </article>

          <article class="service-card">
            <div class="service-icon">🌐</div>
            <h3>Digital Services</h3>
            <p>
              Tell us about your digital service needs
              and we can discuss the available options.
            </p>
          </article>

          <article class="service-card">
            <div class="service-icon">✨</div>
            <h3>Personalized Help</h3>
            <p>
              Share your requirements so we can help
              you understand the next steps.
            </p>
          </article>
        </div>
      </div>
    </section>

    <section class="about" id="about">
      <div class="container about-content">
        <h2>About KS Online Services</h2>
        <p>
          Our goal is to make online support approachable,
          convenient, and easy to understand. We welcome
          inquiries from customers worldwide and aim to
          provide clear communication throughout the process.
        </p>
      </div>
    </section>

    <section class="contact" id="contact">
      <div class="container">
        <div class="contact-card">
          <h2>Let's Connect!</h2>
          <p>
            Have a question or need help with an online
            service? Get in touch with us.
          </p>

          <div class="contact-links">
            <a
              class="button button-primary"
              href="https://wa.me/919927170739"
              target="_blank"
              rel="noopener noreferrer">
              WhatsApp Us
            </a>

            <a
              class="button button-outline"
              href="mailto:ksonlinservices2818@gmail.com">
              Send an Email
            </a>
          </div>

          <a
            class="contact-email"
            href="mailto:ksonlinservices2818@gmail.com">
            ksonlinservices2818@gmail.com
          </a>

          <p style="margin-top: 10px; margin-bottom: 0;">
            Phone: +91 99271 70739
          </p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>
        &copy; <span id="year"></span> KS Online Services.
        All rights reserved.
      </p>
      <p>Here to make online support simpler.</p>
    </div>
  </footer>

  <script>
    document.getElementById("year").textContent =
      new Date().getFullYear();
  </script>

</body>
</html>
