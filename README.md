# Eclectic.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Eclectic</title>
  <link rel="icon" type="image/svg+xml" href="favicon.svg" />
  <style>
    /* Reset */
    *{margin:0;padding:0;box-sizing:border-box;}
    body{font-family:Arial, sans-serif;line-height:1.6;color:#333;background:#f9fafb;}

    /* Navbar */
    header{background:#4f46e5;color:white;padding:1rem;display:flex;justify-content:space-between;align-items:center;position:sticky;top:0;z-index:1000;}
    header img{height:40px;}
    nav a{color:white;text-decoration:none;margin:0 1rem;font-weight:bold;}
    nav a:hover{color:#d1d5db;}

    /* Hero */
    .hero{background:linear-gradient(135deg,#4f46e5,#9333ea);color:white;text-align:center;padding:5rem 2rem;}
    .hero h1{font-size:2.5rem;margin-bottom:1rem;}
    .hero p{font-size:1.2rem;margin-bottom:2rem;}
    .btn{background:#f59e0b;color:white;padding:.8rem 1.5rem;border:none;border-radius:25px;cursor:pointer;font-size:1rem;}
    .btn:hover{background:#d97706;}

    /* Sections */
    section{padding:4rem 2rem;max-width:1200px;margin:auto;}
    h2{text-align:center;margin-bottom:2rem;color:#4f46e5;}

    /* YouTube */
    .youtube iframe{width:100%;height:400px;border:none;border-radius:10px;}

    /* Cards */
    .cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1.5rem;}
    .card{background:white;padding:1.5rem;border-radius:15px;box-shadow:0 4px 10px rgba(0,0,0,0.1);text-align:center;}
    .card h3{margin-bottom:1rem;color:#9333ea;}
    .card p{margin-bottom:1rem;}
    .card .btn{margin-top:auto;}

    /* Signup */
    .signup{text-align:center;background:#eef2ff;padding:3rem;border-radius:15px;}
    .signup input{padding:.8rem;width:250px;border:1px solid #ccc;border-radius:25px;margin-right:.5rem;}
    .signup button{padding:.8rem 1.5rem;border:none;background:#4f46e5;color:white;border-radius:25px;cursor:pointer;}
    .signup button:hover{background:#4338ca;}

    /* Footer */
    footer{background:#1f2937;color:#d1d5db;padding:2rem;text-align:center;margin-top:3rem;}
    footer a{color:#f59e0b;text-decoration:none;}
    footer .socials a{margin:0 .5rem;color:#d1d5db;}
    footer .socials a:hover{color:white;}

    /* Popup */
    #exitPopup{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.6);justify-content:center;align-items:center;}
    #exitPopup .content{background:white;padding:2rem;border-radius:15px;text-align:center;max-width:400px;}
    #exitPopup button{margin-top:1rem;background:#4f46e5;color:white;border:none;padding:.7rem 1.2rem;border-radius:25px;cursor:pointer;}
    #exitPopup button:hover{background:#4338ca;}
  </style>
</head>
<body>

  <!-- Navbar -->
  <header>
    <img src="logo.svg" alt="Eclectic Hub Logo">
    <nav>
      <a href="#home">Home</a>
      <a href="#youtube">YouTube</a>
      <a href="#programs">Programs</a>
      <a href="#affiliate">Affiliates</a>
      <a href="#blog">Blog</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <h1>Welcome to The Eclectic Hub</h1>
    <p>Your one-stop space for Finance, Tech, and Travel insights.</p>
    <button class="btn">Explore Now</button>
  </section>

  <!-- YouTube -->
  <section id="youtube" class="youtube">
    <h2>Latest from Our YouTube Channel</h2>
    <iframe src="https://www.youtube.com/embed?listType=user_uploads&list=CHANNEL_ID" allowfullscreen></iframe>
    <div style="text-align:center;margin-top:1rem;">
      <a href="https://www.youtube.com/@Eclectic-hub" target="_blank" class="btn">Visit Channel</a>
    </div>
  </section>

  <!-- Programs -->
  <section id="programs">
    <h2>Our Programs</h2>
    <div class="cards">
      <div class="card">
        <h3>Finance Growth</h3>
        <p>Learn how to grow and manage wealth effectively.</p>
        <button class="btn">Learn More</button>
      </div>
      <div class="card">
        <h3>Tech Insights</h3>
        <p>Explore the latest in technology and AI tools.</p>
        <button class="btn">Learn More</button>
      </div>
      <div class="card">
        <h3>Travel Hacks</h3>
        <p>Discover cost-saving tips and global destinations.</p>
        <button class="btn">Learn More</button>
      </div>
    </div>
  </section>

  <!-- Affiliate -->
  <section id="affiliate">
    <h2>Affiliate Picks</h2>
    <div class="cards">
      <div class="card">
        <h3>Affiliate Product 1</h3>
        <p>Short description of the affiliate product.</p>
        <a href="#" class="btn">Shop Now</a>
      </div>
      <div class="card">
        <h3>Affiliate Product 2</h3>
        <p>Short description of the affiliate product.</p>
        <a href="#" class="btn">Shop Now</a>
      </div>
    </div>
  </section>

  <!-- Blog -->
  <section id="blog">
    <h2>From the Blog</h2>
    <div class="cards">
      <div class="card">
        <h3>Blog Post Title</h3>
        <p>Preview text for your article...</p>
        <a href="#" class="btn">Read More</a>
      </div>
      <div class="card">
        <h3>Blog Post Title</h3>
        <p>Preview text for your article...</p>
        <a href="#" class="btn">Read More</a>
      </div>
    </div>
  </section>

  <!-- Signup -->
  <section class="signup">
    <h2>Join The Eclectic Hub Community</h2>
    <p>Get updates, tips, and exclusive offers directly to your inbox.</p>
    <form>
      <input type="email" placeholder="Enter your email" required>
      <button type="submit">Join Now</button>
    </form>
  </section>

  <!-- Footer -->
  <footer id="contact">
    <p class="socials">
      <a href="#">Facebook</a> | <a href="#">Twitter</a> | <a href="#">Instagram</a>
    </p>
    <p>Affiliate Disclaimer: Some of the links on this site may be affiliate links. We may earn a commission at no extra cost to you.</p>
    <p>&copy; 2025 The Eclectic Hub. All rights reserved.</p>
  </footer>

  <!-- Exit Popup -->
  <div id="exitPopup">
    <div class="content">
      <h2>Wait! Don’t leave yet</h2>
      <p>Join our community for free insights in Finance, Tech & Travel!</p>
      <button onclick="closePopup()">Close</button>
    </div>
  </div>

  <script>
    // Exit intent popup
    document.addEventListener("mouseleave", function(e){
      if(e.clientY < 10){
        document.getElementById("exitPopup").style.display="flex";
      }
    });
    function closePopup(){
      document.getElementById("exitPopup").style.display="none";
    }

    // Simple form submission (placeholder)
    document.querySelector(".signup form").addEventListener("submit", function(e){
      e.preventDefault();
      alert("Thank you for subscribing!");
    });
  </script>
</body>
</html>
