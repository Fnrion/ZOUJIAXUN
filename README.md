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

<div class="main-content">
  <section id="about">
    <h2>About</h2>

**Student**  
Singapore Management University, School of Computing and Information Systems  
**Pursuing Master of IT in Business (Analytics Track)**  
*Singapore*

---

I am currently a Master’s student at Singapore Management University, specializing in the Analytics Track of the Master of IT in Business (MITB) program. With a background in Business Administration and a deep interest in data-driven decision-making, I am passionate about leveraging data analytics to address complex business challenges.

Previously, I have gained experience in financial analysis and trading, with roles at J.P. Morgan and Gaierpu International Trading Corporation. My professional journey has equipped me with skills in financial data analysis, market research, and strategic decision-making, enabling me to contribute effectively to data-centric roles. At J.P. Morgan, I assisted in consolidating data during a critical period of federal rate hikes, offering insights that supported the fund manager’s investment strategies.

In addition to my financial expertise, I have hands-on experience with analytical tools like Python, R, and Tableau, which I use to uncover meaningful insights from data. I am also keen on exploring the applications of machine learning in business contexts and am committed to continuous learning and development in this field.

My academic and professional experiences have not only refined my technical skills but also deepened my understanding of how data science can drive impactful solutions across industries.
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
