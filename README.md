<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>FAQ ‒ UK International London Beauty School</title>
  <style>
    /* General reset / base styles */
    body, h1, h2, h3, p, ul, li {
      margin: 0;
      padding: 0;
    }
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background-color: #f5f5f5;
      color: #333;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    ul {
      list-style: none;
    }

    /* Container */
    .container {
      width: 90%;
      max-width: 1000px;
      margin: 0 auto;
      padding: 20px;
    }

    /* Header / Navigation */
    header {
      background-color: #ffffff;
      padding: 20px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .nav {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
    }
    .nav .logo {
      font-size: 1.5em;
      font-weight: bold;
      color: #c2185b; /* pinkish / beauty theme color */
    }
    .nav ul {
      display: flex;
      gap: 15px;
    }
    .nav ul li a {
      padding: 8px 12px;
      color: #333;
      transition: color 0.3s;
    }
    .nav ul li a:hover {
      color: #c2185b;
    }

    /* FAQ section */
    .faq-section {
      margin-top: 40px;
      background: #ffffff;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    .faq-section h1 {
      text-align: center;
      margin-bottom: 30px;
      color: #c2185b;
    }
    .faq-item {
      margin-bottom: 20px;
      border-bottom: 1px solid #ddd;
      padding-bottom: 10px;
    }
    .faq-item h3 {
      font-size: 1.2em;
      cursor: pointer;
      position: relative;
      padding-right: 30px;
    }
    .faq-item h3::after {
      content: '+';
      position: absolute;
      right: 0;
      font-size: 1.2em;
      transition: transform 0.3s;
    }
    .faq-item.active h3::after {
      content: '−';
      transform: rotate(180deg);
    }
    .faq-item p {
      display: none;
      margin-top: 10px;
      padding-left: 10px;
      color: #555;
    }

    /* Footer */
    footer {
      margin-top: 40px;
      background-color: #ffffff;
      padding: 20px;
      text-align: center;
      color: #666;
      font-size: 0.9em;
      border-top: 1px solid #ddd;
    }
  </style>
</head>
<body>

  <header>
    <div class="container nav">
      <div class="logo">UK International London Beauty School</div>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About Us</a></li>
        <li><a href="courses.html">Courses</a></li>
        <li><a href="registration.html">Registration</a></li>
        <li><a href="placement.html">Placement</a></li>
        <li><a href="faq.html">FAQ's</a></li>
        <li><a href="contact.html">Contact Us</a></li>
      </ul>
    </div>
  </header>

  <div class="container faq-section">
    <h1>Frequently Asked Questions</h1>

    <div class="faq-item">
      <h3>What courses do you offer?</h3>
      <p>We offer professional courses in Makeup, Hair Styling, Skin Therapy, Nail Art, Cosmetology, and Beauty Therapy. Both short-term and comprehensive long-term programs are available.</p>
    </div>

    <div class="faq-item">
      <h3>Do you provide certification?</h3>
      <p>Yes. All our courses are certified by accredited bodies recognized internationally. We issue certificates upon successful completion of each course.</p>
    </div>

    <div class="faq-item">
      <h3>Where is your institute located?</h3>
      <p>Our main campus is in London, UK. We also have partner centres / branches for practicals depending on the course. Exact location details are provided during registration.</p>
    </div>

    <div class="faq-item">
      <h3>What is the process for enrollment?</h3>
      <p>You can enroll by filling out our online registration form, submitting required documents, and paying the course fee. We provide career counseling to help you choose the right course.</p>
    </div>

    <div class="faq-item">
      <h3>What are the payment options?</h3>
      <p>We accept payments via bank transfer, major credit/debit cards, and online payment platforms. Interest-free installment plans are available for eligible students.</p>
    </div>

    <div class="faq-item">
      <h3>Is there any placement assistance?</h3>
      <p>Yes, we provide 100% placement assistance. Our team helps with portfolio building, mock interviews, and connects you with beauty salons, studios, and industry contacts in London and beyond.</p>
    </div>

    <div class="faq-item">
      <h3>What makes UK International London Beauty School different?</h3>
      <p>We focus on hands-on practical training, latest techniques, real industry exposure, certified trainers, and small batch sizes to ensure personalized attention.</p>
    </div>

  </div>

  <footer>
    © UK International London Beauty School ‒ All Rights Reserved
  </footer>

  <script>
    // JS to enable toggle behavior
    document.addEventListener('DOMContentLoaded', function() {
      const items = document.querySelectorAll('.faq-item h3');
      items.forEach(function(header) {
        header.addEventListener('click', function() {
          const parent = header.parentElement;
          const answer = header.nextElementSibling;
          const isActive = parent.classList.contains('active');
          if (isActive) {
            // close it
            answer.style.display = 'none';
            parent.classList.remove('active');
          } else {
            // close any opened first (optional)
            // items.forEach(h => {
            //   h.parentElement.classList.remove('active');
            //   h.nextElementSibling.style.display = 'none';
            // });
            // open this one
            answer.style.display = 'block';
            parent.classList.add('active');
          }
        });
      });
    });
  </script>

</body>
</html>
