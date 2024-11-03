<!-- Include Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">

<style>
  /* Style for the container */
  .container {
    display: flex;
    align-items: flex-start;
  }

  /* Style for the main content */
  .main-content {
    width: 70%;
    padding-right: 20px;
    font-family: 'Times New Roman', Times, serif;
  }

  /* Style for the sidebar */
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
    font-family: 'Roboto', sans-serif;
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
    background-color: #d0e1ff;
    border-radius: 5px;
    font-weight: bold;
  }

  /* Styling for headings */
  h2 {
    font-weight: bold;
    font-family: 'Roboto', sans-serif;
  }

  /* Custom styles for experience section */
  .job-title {
    font-weight: bold;
  }
  .company-info {
    font-style: italic;
    color: #333;
  }
  .date-info {
    color: #666;
    font-style: italic;
  }
</style>

<div class="container">
  <!-- Main Content Section -->
  <div class="main-content">
    <section id="about">
      <p>Student<br>
      Singapore Management University, School of Computing and Information Systems<br>
      Pursuing Master of IT in Business (Analytics Track)<br>
      <em>Singapore</em></p>
      <hr>
      <p>I am currently a Master’s student at Singapore Management University, specializing in the Analytics Track of the Master of IT in Business (MITB) program. With a background in Business Administration and a deep interest in data-driven decision-making, I am passionate about leveraging data analytics to address complex business challenges.</p>
    </section>

    <section id="experience">
      <h2>Experience</h2>

      <p>
        <span class="job-title">Export Trader</span>, Gaierpu International Trading Corporation<br>
        <span class="company-info">Jiangsu, China</span><br>
        <span class="date-info">Jun 2021 - Aug 2021</span><br>
        Collaborated with a team on inventory checks and customer engagement, securing a bulk order of 10,000 N95 masks and achieving 100% on-time delivery to enhance customer satisfaction.
      </p>

      <p>
        <span class="job-title">Account Assistant</span>, Changzhou Jinbaihe<br>
        <span class="company-info">Jiangsu, China</span><br>
        <span class="date-info">Jun 2022 - Aug 2022</span><br>
        Recorded daily transactions, coordinated financial reporting with department managers, and analyzed statements. Helped increase cash flow by 12% through insights on abnormal data like high receivables.
      </p>
      
      <p>
        <span class="job-title">Assistant Analyst</span>, J.P. Morgan<br>
        <span class="company-info">China (Remote Part-time)</span><br>
        <span class="date-info">Sep 2023 - Nov 2023</span><br>
        Collected financial data during the federal rate hike cycle, consolidating insights in the database. Conducted company research, analyzed market trends, and provided investment recommendations to the fund manager.
      </p>
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

  <!-- Sidebar Section -->
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