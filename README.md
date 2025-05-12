<!DOCTYPE html>
<html lang="en">

<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Siksha - Corporate Training Solutions</title>
 <!-- Google Font -->
 <link href="https://fonts.googleapis.com/css?family=Roboto:400,500,700" rel="stylesheet" />
 <!-- Custom CSS -->
 <style>
 /* CSS Reset and General Styles */
 
 *,
 *::before,
 *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
 }
 
 body {
  font-family: 'Roboto', sans-serif;
  line-height: 1.6;
  color: #2c3e50;
  background-color: #e0f2f1;
  text-align: center;
  font-size: 16px;
 }
 
 a {
  text-decoration: none;
  color: inherit;
  transition: color 0.3s ease;
 }
 
 a:hover {
  color: #004d40;
 }
 
 ul {
  list-style: none;
 }
 
 img {
  max-width: 100%;
  display: block;
 }
 
 /* Utility Classes */
 
 .container {
  width: 90%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 15px;
 }
 
 .btn {
  display: inline-block;
  background-color: #006666;
  color: #fff;
  padding: 10px 20px;
  border-radius: 4px;
  font-weight: bold;
  transition: background-color 0.3s ease;
  border: none;
  cursor: pointer;
  font-size: 1rem;
 }
 
 .btn:hover {
  background-color: #004f4f;
 }
 
 /* Navbar Styles */
 
 .navbar {
  background: #4db6ac;
  border-bottom: 1px solid #80cbc4;
  position: sticky;
  top: 0;
  z-index: 100;
  padding: 1rem 0;
 }
 
 .navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
 }
 
 .navbar .logo {
  font-size: 1.5rem;
  font-weight: 700;
  color: #ffffff;
 }
 
 .nav-list {
  display: flex;
 }
 
 .nav-list li {
  margin-left: 1rem;
 }
 
 .nav-list li a {
  font-weight: 500;
  color: #ffffff;
  display: block;
  padding: 0.5rem;
 }
 
 /* Mobile Menu Toggle */
 
 .menu-toggle {
  display: none;
  flex-direction: column;
  cursor: pointer;
 }
 
 .menu-toggle span {
  height: 3px;
  width: 25px;
  background: #ffffff;
  margin-bottom: 4px;
  border-radius: 2px;
 }
 
 /* Hero Section Styles */
 
 .hero {
  background-image: url('x.jpg');
  background-size: cover;
  background-position: center;
  background-blend-mode: darken;
  background-color: rgba(0, 0, 0, 0.6);
  color: #ffffff;
  padding: 4rem 0;
 }
 
 .hero-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
 }
 
 .hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
 }
 
 .hero p {
  font-size: 1.1rem;
  max-width: 80%;
  margin: 0 auto 1.5rem;
 }
 
 /* Card Section Styles */
 
 .cardsec {
  background-color: #b2dfdb;
  padding: 2rem 0;
 }
 
 .cardsec-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: stretch;
 }
 
 .card-ad {
  background-color: #ffffff;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
  margin-bottom: 1rem;
  width: calc(33% - 2rem);
  min-width: 250px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
 }
 
 .card-ad:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
 }
 
 .image_box {
  width: 80%;
  height: 50%;
  background-color: #e0f2f1;
  overflow: hidden;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
 }
 
 .image_box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s ease-in-out;
 }
 
 .image_box:hover img {
  transform: scale(1.2);
 }
 
 .p_card {
  text-align: center;
  font-size: 0.9rem;
  padding: 1rem;
  color: #555;
 }
 
 /* About Section Styles */
 
 .about {
  background: #ffffff;
  padding: 3rem 0;
 }
 
 .about-container {
  max-width: 800px;
  margin: 0 auto;
 }
 
 .about h1 {
  font-size: 2.2rem;
  margin-bottom: 1.5rem;
 }
 
 .about p {
  font-size: 1.1rem;
  line-height: 1.7;
  margin-bottom: 1rem;
  text-align: left;
 }
 
 /* Features Section Styles */
 
 .features {
  background: #b2dfdb;
  padding: 3rem 0;
 }
 
 .features h2 {
  font-size: 2rem;
  margin-bottom: 1.5rem;
  text-align: center;
 }
 
 .feature-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
 }
 
 .feature {
  background: #ffffff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  margin: 1rem;
  padding: 1.5rem;
  border-radius: 8px;
  width: calc(33% - 2rem);
  min-width: 250px;
  text-align: left;
 }
 
 .feature h3 {
  font-size: 1.4rem;
  margin-bottom: 0.75rem;
 }
 
 .feature p {
  font-size: 1rem;
  line-height: 1.6;
 }
 
 /* Programs Section Styles */
 
 .programs {
  background: #1faba4;
  padding: 3rem 0;
 }
 
 .programs h2 {
  font-size: 2rem;
  margin-bottom: 1.5rem;
  text-align: center;
  color: #ffffff;
 }
 
 .program-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
 }
 
 .program {
  background: #ffffff;
  margin: 1rem;
  padding: 1.5rem;
  border-radius: 8px;
  width: calc(33% - 2rem);
  min-width: 250px;
  text-align: left;
 }
 
 .program h3 {
  font-size: 1.4rem;
  margin-bottom: 0.75rem;
 }
 
 .program p {
  font-size: 1rem;
  line-height: 1.6;
  margin-bottom: 1rem;
 }
 
 /* Challenges Section Styles */
 
 .challenges {
  padding: 3rem 0;
 }
 
 .challenges h2 {
  font-size: 2rem;
  margin-bottom: 1.5rem;
  text-align: center;
 }
 
 .challenges-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 20px;
 }
 
 .column {
  flex: 1 1 300px;
  box-sizing: border-box;
  margin: 10px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
  max-width: 400px;
  min-width: 280px;
  background-color: #f8f8f8;
 }
 
 /* Training Packages Section Styles */
 
 .tp {
  background-color: #1faba4;
  color: #ffffff;
  padding: 3rem 0;
 }
 
 .tp .hero1 {
  text-align: center;
  margin-bottom: 2rem;
 }
 
 .tp .hero1 h2 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
 }
 
 .tp .hero1 p {
  max-width: 700px;
  margin: 0 auto;
  font-size: 1.1rem;
  line-height: 1.6;
 }
 
 .tabs {
  text-align: center;
  margin-bottom: 2rem;
 }
 
 .tabs button {
  background-color: #fff;
  border: 2px solid #006666;
  color: #006666;
  padding: 0.75rem 1.5rem;
  margin: 5px;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s;
 }
 
 .tabs button:hover {
  background-color: #e0f2f2;
 }
 
 .tabs button.active {
  background-color: #006666;
  color: #fff;
 }
 
 .sub-info {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 2rem;
  font-size: 1.1rem;
 }
 
 /* Pricing Cards Styles */
 
 .cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  max-width: 1200px;
  margin: 0 auto;
 }
 
 .card {
  background-color: #fff;
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 20px;
  text-align: center;
  position: relative;
  transition: box-shadow 0.3s ease;
  width: calc(25% - 20px);
  min-width: 250px;
  margin: 10px;
  color: #333;
 }
 
 .card:hover {
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
 }
 
 .card .badge {
  position: absolute;
  top: 20px;
  right: 20px;
  background-color: #008080;
  color: #fff;
  font-size: 0.75rem;
  font-weight: bold;
  padding: 4px 8px;
  border-radius: 4px;
 }
 
 .card h3 {
  margin-bottom: 10px;
  color: #006666;
  font-size: 1.3rem;
 }
 
 .card p {
  font-size: 0.95rem;
  margin-bottom: 20px;
 }
 
 .card ul {
  list-style: none;
  text-align: left;
  margin: 20px 0;
  padding: 0;
 }
 
 .card ul li {
  margin: 8px 0;
  position: relative;
  padding-left: 25px;
  font-size: 0.9rem;
 }
 
 .card ul li::before {
  content: "✔";
  color: #006666;
  position: absolute;
  left: 0;
 }
 
 .price {
  font-size: 1.2rem;
  color: #006666;
  font-weight: bold;
  margin-bottom: 15px;
 }
 
 /* Footer Styles */
 
 .footer {
  background: #004d40;
  color: #ffffff;
  padding: 1rem 0;
  text-align: center;
 }
 
 /* Dropdown (Details/Summary) Styles */
 
 details summary {
  font-size: 1.2rem;
  font-weight: bold;
  cursor: pointer;
  padding: 5px;
  background: #eee;
  border-radius: 5px;
  outline: none;
  text-align: left;
 }
 
 details[open] summary {
  background: #ddd;
 }
 
 details ul {
  list-style-type: disc;
  margin-left: 20px;
  margin-top: 10px;
 }
 
 details li {
  margin: 5px 0;
 }
 
 /* Media Queries for Responsiveness */
 
 @media (max-width: 767px) {
  body {
   font-size: 14px;
  }
 
  .navbar {
   padding: 0.5rem 0;
  }
 
  .navbar .logo {
   font-size: 1.2rem;
  }
 
  .nav-list {
   display: none;
   flex-direction: column;
   background: #4db6ac;
   position: absolute;
   top: 60px;
   right: 0;
   width: 100%;
   box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
   text-align: center;
  }
 
  .nav-list.active {
   display: flex;
  }
 
  .nav-list li {
   margin: 0;
   padding: 0.75rem;
   border-bottom: 1px solid #80cbc4;
  }
 
  .nav-list li a {
   display: block;
   width: 100%;
  }
 
  .menu-toggle {
   display: flex;
  }
 
  .hero {
   padding: 2rem 0;
  }
 
  .hero h1 {
   font-size: 1.7rem;
  }
 
  .hero p {
   font-size: 1rem;
  }
 
  .cardsec-container {
   flex-direction: column;
  }
 
  .card-ad {
   width: 90%;
   margin-bottom: 1.5rem;
  }
 
  .feature-container,
  .program-container {
   flex-direction: column;
  }
 
  .feature,
  .program {
   width: 90%;
   margin-bottom: 1.5rem;
  }
 
  .challenges-container {
   flex-direction: column;
  }
 
  .column {
   width: 90%;
   margin-bottom: 1.5rem;
  }
 
  .cards {
   flex-direction: column;
  }
 
  .card {
   width: 90%;
   margin-bottom: 1.5rem;
  }
 }
 
 /* Tablet Screens */
 
 @media (min-width: 768px) and (max-width: 1023px) {
  .cardsec-container {
   flex-wrap: wrap;
  }
 
  .card-ad {
   width: calc(50% - 2rem);
   margin-bottom: 1rem;
  }
 
  .feature-container,
  .program-container {
   justify-content: space-around;
  }
 
  .feature,
  .program {
   width: calc(50% - 2rem);
   margin-bottom: 1rem;
  }
 
  .challenges-container {
   justify-content: space-around;
  }
 
  .column {
   width: calc(50% - 2rem);
   margin-bottom: 1rem;
  }
 
  .cards {
   flex-wrap: wrap;
  }
 
  .card {
   width: calc(50% - 20px);
   margin-bottom: 1rem;
  }
 }
 
 /* Larger Desktop Screens */
 
 @media (min-width: 1200px) {
  .hero h1 {
   font-size: 3rem;
  }
 }
 </style>
</head>

<body>
 <!-- Navbar -->
 <nav class="navbar">
  <div class="container navbar-container">
   <a href="#" class="logo">𝒮𝒾𝓀𝓈𝒽𝒶</a>
   <div class="menu-toggle" id="mobile-menu">
    <span></span>
    <span></span>
    <span></span>
   </div>
   <ul class="nav-list">
    <li><a href="#hero">Home</a></li>
    <li><a href="#features">Key Features</a></li>
    <li><a href="#programs">Training Programs</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="login.html">Log In</a></li>
   </ul>
  </div>
 </nav>

 <!-- Hero Section -->
 <section class="hero" id="hero">
  <div class="container hero-container">
   <h1>Transform Your Workforce with Expert Training</h1>
   <p>Experience instructor-led learning that transforms corporate training, providing tailored solutions for your
    business
    needs anytime, anywhere.</p>
   <button class="btn">Learn More</button>
  </div>
 </section>

 <!-- Card Section -->
 <section class="cardsec">
  <div class="container cardsec-container">
   <div class="card-ad">
    <div class="image_box">
     <img src="https://babafaridgroup.edu.in/assets/img/bfgi/importance-of-skill-development.jpg"
      alt="Skill Development">
    </div>
    <p class="p_card">
     Improve your team's capabilities and knowledge through focused skill development initiatives.
    </p>
   </div>

   <div class="card-ad">
    <div class="image_box">
     <img src="https://thumbs.dreamstime.com/b/effective-chart-keywords-icons-48965289.jpg" alt="Effective">
    </div>
    <p class="p_card">
     Maximize productivity and achieve better outcomes with our effective training strategies.
    </p>
   </div>

   <div class="card-ad">
    <div class="image_box">
     <img src="https://www.lecansolutions.com/images/Customized-Solutions.jpg" alt="Customized Service">
    </div>
    <p class="p_card">
     Benefit from training programs that are specifically customized to meet your organization's unique needs.
    </p>
   </div>
  </div>
 </section>

 <!-- About Section -->
 <section class="about" id="about" style="background-color: #1FABA4;">
  <div class="container about-container">
   <h1>About Siksha</h1>
   <!-- Increased width by adjusting padding and max-width -->
   <div
    style="text-align: center; background-color: white; padding-left: 50px; padding-right: 50px; height: auto; max-width: 100%;">
    <p>
     At Siksha, we're not just another training provider; we're your strategic partner in workforce transformation.
     In today's rapidly evolving business landscape, continuous learning is no longer a luxury—it's a necessity.
     That's why we've made it our mission to empower organizations and individuals with the skills and knowledge
     they need to thrive.
    </p>

    <p>
     We take a holistic approach to learning and development, combining cutting-edge methodologies, industry best
     practices, and a deep understanding of your unique business challenges. Whether you're looking to upskill your
     workforce, drive innovation, or enhance leadership capabilities, we'll work closely with you to design and
     deliver customized training solutions that align with your goals and deliver measurable results.
    </p>

    <p>
     Our team of experienced trainers and consultants are passionate about helping you unlock your full potential.
     We're committed to creating engaging and impactful learning experiences that inspire growth, foster collaboration,
     and drive business success.
    </p>

    <p>
     Join us on a journey of continuous improvement and strategic learning. Let Siksha be your guide to a brighter,
     more successful future.
    </p>
   </div>
  </div>
 </section>

 <!-- Features Section -->
 <section class="features" id="features">
  <div class="container">
   <h2>Our Key Features</h2>
   <div class="feature-container">
    <div class="feature">
     <h3>Expert-Led Training</h3>
     <p>Engage with industry experts who deliver top-notch training sessions, bringing real-world experience to the
      learning environment.</p>
    </div>
    <div class="feature">
     <h3>Tailored Programs</h3>
     <p>Customized training that aligns with your company's goals and specific needs, ensuring relevance and
      impact.</p>
    </div>
    <div class="feature">
     <h3>Flexible Learning</h3>
     <p>Learn anytime, anywhere with our accessible training platform, designed to fit the schedules of busy
      professionals.</p>
    </div>
   </div>
  </div>
 </section>

 <!-- Programs Section -->
 <section class="programs" id="programs">
  <div class="container">
   <h2>Training Programs</h2>
   <div class="program-container">
    <div class="program">
     <h3>Corporate Leadership</h3>
     <p>Develop leadership skills that drive business success and inspire teams to achieve common goals.</p>
     <button class="btn">Enroll Now</button>
    </div>
    <div class="program">
     <h3>Technical Mastery</h3>
     <p>Enhance technical expertise with hands-on training and real-world applications to stay ahead in your
      industry.</p>
     <button class="btn">Enroll Now</button>
    </div>
    <div class="program">
     <h3>Soft Skills Development</h3>
     <p>Boost communication, collaboration, and problem-solving skills to improve workplace dynamics and
      effectiveness.</p>
     <button class="btn">Enroll Now</button>
    </div>
   </div>
  </div>
 </section>

 <!-- Challenges Section -->
 <section class="challenges">
  <div class="container">
   <h2 style="padding-top: 2em;">Training Challenges</h2>
   <div class="challenges-container">
    <div class="column">
     <details>
      <summary>Large Organization Challenges</summary>
      <ul>
       <li>Scale and Complexity</li>
       <li>Diverse Learning Needs</li>
       <li>Non-centralized Training Administration</li>
       <li>Content Update Delays</li>
       <li>Scheduling Conflicts</li>
      </ul>
     </details>
    </div>

    <div class="column">
     <details>
      <summary>Common Challenges</summary>
      <ul>
       <li>Logistical Complications</li>
       <li>Lack of In-house Corporate Trainers</li>
       <li>Over-reliance on Multiple Training Vendors</li>
       <li>Consistency in Training Quality</li>
       <li>Content Update Delays</li>
       <li>Training Across Geographies Leading to Coordination Delays</li>
      </ul>
     </details>
    </div>

    <div class="column">
     <details>
      <summary>Small & Medium Business Challenges</summary>
      <ul>
       <li>Vendor Reliability</li>
       <li>Lack of Training Infrastructure</li>
       <li>Resources and Funds</li>
       <li>Training in Multiple Geographies</li>
       <li>Customization Challenges</li>
       <li>Budget Constraints</li>
       <li>Cultural Resistance</li>
      </ul>
     </details>
    </div>
   </div>
  </div>
 </section>

 <!-- Training Packages Section -->
 <section class="tp">
  <div class="container">
   <section class="hero1">
    <h2>Training Packages Tailored for Diverse Organizational Needs</h2>
    <p>
     One-of-its-kind instructor-led corporate training packages address
     the critical upskilling challenges of organizations of all sizes and scale.
    </p>
   </section>

   <!-- Tabs / Toggle Buttons -->
   <div class="tabs">
    <button class="active">Technical Training</button>
    <button>Non-Technical Training</button>
    <button>All Included</button>
   </div>

   <!-- Sub-Headline / Additional Info -->
   <div class="sub-info">
    Boost your team's expertise with over 1000+ cutting-edge instructor-led
    Technical training programs.
   </div>

   <!-- Pricing Cards -->
   <div class="cards">
    <!-- Starter Card -->
    <div class="card">
     <h3>Starter</h3>
     <p>120 licenses</p>
     <p>Tailor-Made Licenses with Our Exclusive Training Package</p>
     <ul>
      <li>24 hours of training</li>
      <li>Basic Q&A sessions</li>
      <li>Tailored for SMBs</li>
     </ul>
     <div class="price">$499</div>
     <a href="#" class="btn">View Package</a>
    </div>

    <!-- Growth Card -->
    <div class="card">
     <h3>Growth</h3>
     <p>320 licenses</p>
     <p>Tailor-Made Licenses with Our Exclusive Training Package</p>
     <ul>
      <li>40 hours of training</li>
      <li>Live Q&A and support</li>
      <li>Ideal for growing SMBs</li>
     </ul>
     <div class="price">$999</div>
     <a href="#" class="btn">View Package</a>
    </div>

    <!-- Enterprise Card -->
    <div class="card">
     <h3>Enterprise</h3>
     <p>800 licenses</p>
     <p>Tailor-Made Licenses with Our Exclusive Training Package</p>
     <ul>
      <li>400 hours of training</li>
      <li>Dedicated account manager</li>
      <li>In-depth performance reports</li>
     </ul>
     <div class="price">$1,999</div>
     <a href="#" class="btn">View Package</a>
    </div>

    <!-- Custom Card -->
    <div class="card">
     <h3>Custom</h3>
     <p>Unlimited licenses</p>
     <p>Tailor-Made Licenses with Our Exclusive Training Package</p>
     <ul>
      <li>Unlimited training hours</li>
      <li>24/7 dedicated support</li>
      <li>Fully customizable solutions</li>
     </ul>
     <div class="price">Contact Us</div>
     <a href="#" class="btn">View Package</a>
    </div>
   </div>
  </div>
 </section>

 <!-- Footer -->
 <footer class="footer" id="contact">
  <p>© 2025 Siksha. All rights reserved.</p>
 </footer>

 <!-- JavaScript -->
 <script>
 // Mobile Menu Toggle
 document.getElementById('mobile-menu').addEventListener('click', function() {
  document.querySelector('.nav-list').classList.toggle('active');
 });
 </script>
</body>

</html>
