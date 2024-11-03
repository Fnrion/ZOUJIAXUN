<!-- Include Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap" rel="stylesheet">

<style>
  /* Style for the container */
  .container {
    display: flex;
    align-items: flex-start;
  }
  /* Style for the main content to provide enough space */
  .main-content {
    width: 70%;
    padding-right: 20px;
    font-family: 'Times New Roman', Times, serif;
  }
  /* Style for the sidebar to fix its position on the right */
  .sidebar {
    width: 25%;
    background-color: #f0f4f8;
    padding: 20px;
    text-align: center;
    position: fixed;
    right: 0;
    top: 0;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow-y: auto;
  }
  /* Style for sidebar links */
  .sidebar-link {
    color: #333;
    text-decoration: none;
    padding: 5px;
    display: block;
    transition: background-color 0.3s;
  }
  /* Style for the active link */
  .sidebar-link.active {
    background-color: #d0e1ff; /* Highlight color */
    border-radius: 5px;
    font-weight: bold;
  }
</style>

<div class="container">
  <!-- Main Content Section -->
  <div class="main-content">
    <section id="about">
      <p><strong>Student</strong><br>
      Singapore Management University, School of Computing and Information Systems<br>
      <strong>Pursuing Master of IT in Business (Analytics Track)</strong><br>
      <em>Singapore</em></p>

      <hr>

      <p>I am currently a Master’s student at Singapore Management University, specializing in the Analytics Track of the Master of IT in Business (MITB) program. Also, with a background in Business Administration and a deep interest in data-driven decision-making, I am passionate about leveraging data analytics to address complex business challenges.</p>

    </section>

    <section id="experience">
      <h2>Experience</h2>
      <!-- Experience content here -->
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <!-- Projects content here -->
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <!-- Skills content here -->
    </section>

    <section id="publication">
      <h2>Publication</h2>
      <!-- Publication content here -->
    </section>
  </div>

  <!-- Sidebar Section with Fixed Position and Centered Content -->
  <div class="sidebar">
    <img src="profile.jpg" width="180px" alt="Profile Picture" style="border-radius: 50%; margin-bottom: 10px;">
    <h2>Jiaxun Zou</h2>
    <p><em>Whole life unshaken</em></p>

    <!-- Icons for Email, LinkedIn, and GitHub -->
    <div style="margin: 10px 0;">
      <a href="mailto:connect@zoujiaxun.com" style="margin-right: 10px; color: #333;">
        <i class="fas fa-envelope" style="font-size: 24px;"></i>
      </a>
      <a href="https://www.linkedin.com/in/zoujiaxun" style="margin-right: 10px; color: #333;">
        <i class="fab fa-linkedin" style="font-size: 24px;"></i>
      </a>
      <a href="https://github.com/Fnrion" style="color: #333;">
        <i class="fab fa-github" style="font-size: 24px;"></i>
      </a>
    </div>

    <!-- Sidebar Navigation Links -->
    <ul style="list-style: none; padding: 0; text-align: center;">
      <li><a href="#about" class="sidebar-link">About</a></li>
      <li><a href="#experience" class="sidebar-link">Experience</a></li>
      <li><a href="#projects" class="sidebar-link">Projects</a></li>
      <li><a href="#skills" class="sidebar-link">Skills</a></li>
      <li><a href="#publication" class="sidebar-link">Publication</a></li>
    </ul>
  </div>
</div>

<!-- JavaScript to Highlight Active Section in Sidebar -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const sections = document.querySelectorAll("section");
    const sidebarLinks = document.querySelectorAll(".sidebar-link");

    // Function to clear all active classes
    function clearActiveLinks() {
      sidebarLinks.forEach(link => link.classList.remove("active"));
    }

    // Function to highlight the current section's sidebar link
    function highlightCurrentSection() {
      sections.forEach((section, index) => {
        const sectionTop = section.getBoundingClientRect().top;
        if (sectionTop <= window.innerHeight / 2 && sectionTop >= 0) {
          clearActiveLinks();
          sidebarLinks[index].classList.add("active");
        }
      });
    }

    // Run highlightCurrentSection on scroll
    window.addEventListener("scroll", highlightCurrentSection);
  });
</script>