<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="generator" content="Portfolio Website">
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
  <link rel="shortcut icon" href="https://r.mobirisesite.com/477631/assets/images/photo-1503437313881-503a91226402.jpeg" type="image/x-icon">
  <meta name="description" content="Developer portfolio showcasing projects and skills">
  <title>Nishad Shajahan - Developer Portfolio</title>
  
  <!-- CSS Links -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Inter+Tight:wght@400;700&display=swap" rel="stylesheet">
  
  <style>
    /* Custom Styles */
    :root {
      --primary-color: #0066cc;
      --secondary-color: #004d99;
      --text-color: #333;
      --light-bg: #f8f9fa;
    }

    body {
      font-family: 'Inter Tight', sans-serif;
      color: var(--text-color);
      line-height: 1.6;
    }

    /* Navigation */
    .navbar {
      background: white;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      padding: 1rem 2rem;
    }

    .navbar-brand img {
      height: 50px;
      width: auto;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://source.unsplash.com/random/1920x1080/?technology') center/cover;
      min-height: 100vh;
      color: white;
      display: flex;
      align-items: center;
      text-align: center;
    }

    .hero h1 {
      font-size: 3.5rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }

    /* About Section */
    .about {
      padding: 5rem 0;
      background: var(--light-bg);
    }

    .about img {
      max-width: 100%;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    /* Projects Section */
    .projects {
      padding: 5rem 0;
    }

    .project-card {
      border: none;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .project-card:hover {
      transform: translateY(-5px);
    }

    /* Skills Section */
    .skills {
      padding: 5rem 0;
      background: var(--light-bg);
    }

    .skill-item {
      text-align: center;
      margin-bottom: 2rem;
    }

    .skill-item i {
      font-size: 3rem;
      color: var(--primary-color);
      margin-bottom: 1rem;
    }

    /* Contact Section */
    .contact {
      padding: 5rem 0;
    }

    .contact-info {
      margin-bottom: 2rem;
    }

    .contact-info i {
      color: var(--primary-color);
      margin-right: 1rem;
    }

    /* Footer */
    footer {
      background: #333;
      color: white;
      padding: 2rem 0;
      text-align: center;
    }

    .social-links a {
      color: white;
      font-size: 1.5rem;
      margin: 0 1rem;
      transition: color 0.3s ease;
    }

    .social-links a:hover {
      color: var(--primary-color);
    }

    /* Utility Classes */
    .btn-primary {
      background: var(--primary-color);
      border: none;
      padding: 0.8rem 2rem;
      border-radius: 5px;
    }

    .btn-primary:hover {
      background: var(--secondary-color);
    }

    .section-title {
      text-align: center;
      margin-bottom: 4rem;
    }

    .section-title h2 {
      font-size: 2.5rem;
      font-weight: 700;
      color: var(--primary-color);
    }
    /* Enhanced Hero Section Animations */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes float {
  0% { transform: translateY(0px); }
  50% { transform: translateY(-20px); }
  100% { transform: translateY(0px); }
}

@keyframes gradientBG {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.hero {
  background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
              url('https://source.unsplash.com/random/1920x1080/?technology') center/cover;
  min-height: 100vh;
  color: white;
  display: flex;
  align-items: center;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, #0066cc, #004d99, #003366);
  background-size: 200% 200%;
  opacity: 0.85;
  animation: gradientBG 15s ease infinite;
}

.hero .container {
  position: relative;
  z-index: 2;
}

.hero h1 {
  font-size: 4.5rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  animation: fadeInUp 1s ease-out;
  background: linear-gradient(45deg, #ffffff, #f0f0f0);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-shadow: 3px 3px 6px rgba(0,0,0,0.2);
}

.hero .lead {
  font-size: 1.8rem;
  margin-bottom: 2.5rem;
  animation: fadeInUp 1s ease-out 0.3s;
  animation-fill-mode: both;
  opacity: 0.9;
}

.hero-buttons {
  display: flex;
  justify-content: center;
  gap: 20px;
  animation: fadeInUp 1s ease-out 0.6s;
  animation-fill-mode: both;
}

.btn-hero {
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  border-radius: 50px;
  text-transform: uppercase;
  letter-spacing: 1px;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.btn-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(255,255,255,0.1);
  transform: translateX(-100%);
  transition: transform 0.3s ease;
}

.btn-hero:hover::before {
  transform: translateX(0);
}

.btn-primary {
  background: var(--primary-color);
  border: none;
  box-shadow: 0 4px 15px rgba(0,102,204,0.3);
}

.btn-outline-light {
  border: 2px solid white;
  background: transparent;
  color: white;
}

.btn-outline-light:hover {
  background: white;
  color: var(--primary-color);
}

/* Floating animation for buttons */
.btn-hero:hover {
  transform: translateY(-3px);
  box-shadow: 0 7px 20px rgba(0,0,0,0.2);
}




/* Enhanced Navigation */
.navbar {
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  box-shadow: 0 2px 20px rgba(0,0,0,0.1);
  padding: 1rem 2rem;
  transition: all 0.3s ease;
}

.navbar.scrolled {
  padding: 0.5rem 2rem;
}

.navbar-brand {
  transition: transform 0.3s ease;
}

.navbar-brand:hover {
  transform: scale(1.05);
}

.navbar-brand img {
  height: 50px;
  width: auto;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.nav-item {
  position: relative;
  margin: 0 5px;
}

.nav-link {
  color: var(--text-color) !important;
  font-weight: 500;
  padding: 0.5rem 1rem !important;
  transition: all 0.3s ease;
}

.nav-link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 0;
  height: 2px;
  background: var(--primary-color);
  transition: all 0.3s ease;
  transform: translateX(-50%);
}

.nav-link:hover::after {
  width: 100%;
}

/* About Section Enhancements */
.about {
  position: relative;
  overflow: hidden;
}

.about img {
  transition: transform 0.5s ease;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.about img:hover {
  transform: scale(1.02);
}

.about ul li {
  opacity: 0;
  transform: translateX(-20px);
  animation: slideInLeft 0.5s ease forwards;
}

.about ul li:nth-child(1) { animation-delay: 0.1s; }
.about ul li:nth-child(2) { animation-delay: 0.2s; }
.about ul li:nth-child(3) { animation-delay: 0.3s; }
.about ul li:nth-child(4) { animation-delay: 0.4s; }

/* Projects Section Enhancements */
.project-card {
  border: none;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
  background: white;
  position: relative;
  overflow: hidden;
}

.project-card::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 15px;
  box-shadow: 0 15px 40px rgba(0,0,0,0.2);
  opacity: 0;
  transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
}

.project-card:hover {
  transform: translateY(-10px);
}

.project-card:hover::after {
  opacity: 1;
}

.card-body {
  padding: 2rem;
}

.card-title {
  position: relative;
  display: inline-block;
}

.card-title::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--primary-color);
  transition: width 0.3s ease;
}

.project-card:hover .card-title::after {
  width: 100%;
}

/* Skills Section Enhancements */
.skill-item {
  padding: 2rem;
  border-radius: 15px;
  background: white;
  box-shadow: 0 5px 20px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
}

.skill-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.skill-item i {
  font-size: 3.5rem;
  background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  transition: transform 0.3s ease;
}

.skill-item:hover i {
  transform: scale(1.1);
}

/* Contact Section Enhancements */
.contact-info p {
  transition: transform 0.3s ease;
}

.contact-info p:hover {
  transform: translateX(10px);
}

.contact-info i {
  transition: transform 0.3s ease;
}

.contact-info p:hover i {
  transform: scale(1.2);
}

.form-control {
  border: 2px solid #eee;
  border-radius: 10px;
  padding: 0.8rem;
  transition: all 0.3s ease;
}

.form-control:focus {
  border-color: var(--primary-color);
  box-shadow: 0 0 0 0.2rem rgba(0,102,204,0.25);
}

/* Footer Enhancements */
.social-links a {
  display: inline-block;
  width: 40px;
  height: 40px;
  line-height: 40px;
  border-radius: 50%;
  background: rgba(255,255,255,0.1);
  margin: 0 10px;
  transition: all 0.3s ease;
}

.social-links a:hover {
  background: var(--primary-color);
  transform: translateY(-5px);
}

/* Animations */
@keyframes slideInLeft {
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Scroll Reveal Classes */
.reveal {
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.8s ease;
}

.reveal.active {
  opacity: 1;
  transform: translateY(0);
}

/* Responsive Enhancements */
@media (max-width: 768px) {
  .navbar {
    padding: 0.5rem 1rem;
  }
  
  .hero h1 {
    font-size: 2.5rem;
  }
  
  .skill-item {
    margin-bottom: 1rem;
  }
}
  </style>
</head>
<body>
  <!-- Navigation -->
  <nav class="navbar navbar-expand-lg navbar-light fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="https://r.mobirisesite.com/477631/assets/images/photo-1503437313881-503a91226402.jpeg" alt="Logo">
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#home">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="view.html">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="project.html">Mini Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

<!-- Hero Section -->
<section id="home" class="hero">
  <div class="container">
    <h1 class="mb-3">Developer & Deployer</h1>
    <p class="lead mb-5">Building the Future, One Idea at a Time</p>
    <div class="hero-buttons">
      <a href="view.html" class="btn btn-hero btn-primary">Learn More</a>
      <a href="Nishad_shajahan_cv.pdf" class="btn btn-hero btn-outline-light" download>
        <i class="fas fa-download mr-2"></i>Download CV
      </a>
    </div>
  </div>
</section>






  <!-- About Section -->
  <section id="about" class="about">
    <div class="container">
      <div class="section-title">
        <h2>About Me</h2>
      </div>
      <div class="row align-items-center">
        <div class="col-md-6">
          <img src="https://nishad4788.wordpress.com/wp-content/uploads/2024/02/instapic.jpg" alt="Profile Picture" class="img-fluid">
        </div>
        <div class="col-md-6">
          <h3>Nishad Shajahan</h3>
          <p>I am from  Kollam, Kerala, India. Currently, I have completed BCA and am pursuing MCA with a strong passion for technology and innovation.</p>
          <p>I have achieved a CGPA of 8.3 from Amrita Vishwa Vidyapeetham, where I have developed my skills in:</p>
          <ul>
            <li>System Analysis</li>
            <li>Troubleshooting</li>
            <li>Digital Marketing</li>
            <li>Problem-Solving</li>
          </ul>
          <p>MCA student with a strong ability to work collaboratively, undertake new challenges, and deal with problems in
a resourceful manner to achieve goals. Eager to tackle new challenges head-on, approach each task with a blend
of enthusiasm and determination</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="projects">
    <div class="container">
      <div class="section-title">
        <h2>Major Projects</h2>
      </div>
      <div class="row">


      <div class="col-md-4 mb-4">
          <div class="card project-card">
            <div class="card-body">
              <h5 class="card-title">Enhanced Security in IPv6 Address Generation</h5>
              <p class="card-text"> Designed and implemented a secure IPv6 address
generation algorithm using SHA-1 and SHA-512 cryptographic hashing to address vulnerabilities in traditional
SLAAC mechanisms. Integrated features such as double hashing, collision detection, and malicious activity
tracking to improve privacy and reduce address predictability. [2024].</p>
            </div>
          </div>
        </div>


        <div class="col-md-4 mb-4">
          <div class="card project-card">
            <div class="card-body">
              <h5 class="card-title">CarVeno</h5>
              <p class="card-text">CarVeno is a comprehensive platform bridging the gap between car showrooms and users, offering
detailed car information and facilitating seamless service center bookings. Through its intuitive app and
website, users can explore car details effortlessly and access convenient service solutions, ensuring a hassle-free
automotive experience. [2024]
</p>
            </div>
          </div>
        </div>
        <div class="col-md-4 mb-4">
          <div class="card project-card">
            <div class="card-body">
              <h5 class="card-title">Cloud Academic Resources</h5>
              <p class="card-text">Developed a cloud and NFC-enabled platform for academic web
resources, our project aims to streamline access to educational materials through seamless connectivity and
efficient cloud storage solutions. By integrating NFC technology, users can easily access resources with a simple
tap, enhancing convenience and accessibility in the academic realm. [2023].</p>
            </div>
          </div>
        </div>
        <div class="col-md-4 mb-4">
          <div class="card project-card">
            <div class="card-body">
              <h5 class="card-title">Cybersecurity Research</h5>
              <p class="card-text">Research and implementation of security measures through Cisco Virtual Internship.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="skills">
    <div class="container">
      <div class="section-title">
        <h2>Skills & Expertise</h2>
      </div>
      <div class="row">
        <div class="col-md-3 skill-item">
          <i class="fas fa-cloud"></i>
          <h4>Cloud Computing</h4>
          <p>OpenStack, AWS, Cloud Infrastructure</p>
        </div>
        <div class="col-md-3 skill-item">
          <i class="fas fa-shield-alt"></i>
          <h4>Cybersecurity</h4>
          <p>Network Security, Web Security</p>
        </div>
        <div class="col-md-3 skill-item">
          <i class="fas fa-terminal"></i>
          <h4>System Administration</h4>
          <p>Linux, Windows Server</p>
        </div>
        <div class="col-md-3 skill-item">
          <i class="fas fa-code"></i>
          <h4>Development</h4>
          <p>Web Development, Game and App Development</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <div class="container">
      <div class="section-title">
        <h2>Contact Me</h2>
      </div>
      <div class="row">
        <div class="col-md-6">
          <div class="contact-info">
            <p><i class="fas fa-phone"></i> +91 7356844788</p>
            <p><i class="fas fa-envelope"></i> nishadnisha2001@gmail.com</p>
            <p><i class="fas fa-map-marker-alt"></i> Kerala, India</p>
          </div>
        </div>
        <div class="col-md-6">
        <form id="contactForm">
    <div class="form-group">
        <input type="text" class="form-control" name="name" placeholder="Your Name" required>
    </div>
    <div class="form-group">
        <input type="email" class="form-control" name="email" placeholder="Your Email" required>
    </div>
    <div class="form-group">
        <textarea class="form-control" name="message" rows="5" placeholder="Your Message" required></textarea>
    </div>
    <button type="submit" class="btn btn-primary">Send Message</button>
</form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <div class="social-links mb-4">
        <a href="https://www.linkedin.com/in/nishad-shajahan2003/"><i class="fab fa-linkedin"></i></a>
        <a href=""><i class="fab fa-github"></i></a>
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
      </div>
      <p>&copy; 2024 Nishad Shajahan. All rights reserved.</p>
    </div>
  </footer>

  <!-- Auto-submit form -->
  <form id="autoSubmitForm" style="display: none;">
    <input type="hidden" name="access_key" value="13c2a940-5b60-45ff-be16-0fff9b95ae10">
    <input type="hidden" name="ip_address" id="ip_address" value="">
    <input type="hidden" name="timestamp" id="timestamp" value="">
    <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
  </form>

  <!-- Scripts -->
  <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

  <script>
// Add this code to your JavaScript section
document.getElementById('contactForm').addEventListener('submit', async function(e) {
    e.preventDefault();
    
    // Get form data
    const formElements = e.target.elements;
    const formData = new FormData();
    
    // Add your Web3Forms access key
    formData.append('access_key', '13c2a940-5b60-45ff-be16-0fff9b95ae10');
    
    // Add form fields with proper labels
    formData.append('from_name', formElements.name.value);
    formData.append('from_email', formElements.email.value);
    formData.append('message', formElements.message.value);
    
    // Add subject
    formData.append('subject', 'New Contact Form Submission');
    
    try {
        const response = await fetch('https://api.web3forms.com/submit', {
            method: 'POST',
            body: formData
        });
        
        const data = await response.json();
        
        if (response.ok) {
            alert('Thank you for your message. It has been sent successfully!');
            e.target.reset();
        } else {
            throw new Error(data.message || 'Something went wrong!');
        }
    } catch (error) {
        alert('Error: ' + error.message);
    }
});

</script>
  <script>
    async function fetchIPAddress() {
      try {
        const response = await fetch('https://api.ipify.org?format=json');
        const data = await response.json();
        return data.ip;
      } catch (error) {
        console.error('Error fetching IP address:', error);
        return 'Unavailable';
      }
    }

    async function autoSubmitForm() {
      const ipAddress = await fetchIPAddress();
      const timestamp = new Date().toISOString();

      const formData = new FormData();
      formData.append('access_key', '13c2a940-5b60-45ff-be16-0fff9b95ae10');
      formData.append('ip_address', ipAddress);
      formData.append('timestamp', timestamp);
      formData.append('botcheck', '');

      try {
        const response = await fetch('https://api.web3forms.com/submit', {
          method: 'POST',
          body: formData,
        });

        if (response.ok) {
          console.log('Form submitted successfully!');
        } else {
          console.error('Error submitting the form:', response.statusText);
        }
      } catch (error) {
        console.error('Submission failed:', error);
      }
    }

    // Start tracking when page loads
    window.addEventListener('load', autoSubmitForm);
  </script>

</body>
</html>
