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
      <p><strong>Student</strong><br>
      <strong>Singapore Management University, School of Computing and Information Systems</strong><br>
      <strong>Pursuing Master of IT in Business (Analytics Track)</strong><br>
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

  <div style="margin-bottom: 20px;">
    <h3>Illegal Fish Company Business Activity Analysis (R)</h3>
    <a href="https://isss608-ay2022-23t2-jiaxunzou.netlify.app/" target="_blank">
      <img src="Visual.png" alt="Illegal Fish Company Project Screenshot" style="width:100%; max-width:600px; border-radius:10px; margin-top:10px;">
    </a>
    <p>Used Shiny to develop an interactive visual analytics tool to analyze and monitor corporate networks of fishery companies potentially involved in illegal, unreported, and unregulated (IUU) fishing activities. Processed a knowledge graph with data on companies, owners, employees, and financial status, transforming activities (nodes) and relationships (edges) into a structure suitable for network analysis. Utilized Centrality Analysis (Degree and Betweenness Centrality) to detect key entities with significant influence within the network, revealing ownership structures and transactional connections indicative of control.</p>
  </div>

  <div style="margin-bottom: 20px;">
    <h3>IBM Employee Estimated Value Analysis (Python)</h3>
    <p>Created a data-driven model to optimize EEV (Employee Estimated Value) for IBM by identifying high-impact factors affecting employee satisfaction. Implemented a Random Forest classifier to identify "at-risk" employees based on factors like job role, performance score, and satisfaction levels. Utilized K-means clustering to segment employees into distinct groups based on behavior patterns, tenure, and satisfaction scores, enabling targeted interventions for different employee profiles.</p>
  </div>
</section>

  <div>
    <h3>IBM Employee Estimated Value Analysis (Python)</h3>
    <p>Created a data-driven model to optimize EEV (Employee Estimated Value) for IBM by identifying high-impact factors affecting employee satisfaction. Implemented a Random Forest classifier to identify "at-risk" employees based on factors like job role, performance score, and satisfaction levels. Utilized K-means clustering to segment employees into distinct groups based on behavior patterns, tenure, and satisfaction scores, enabling targeted interventions for different employee profiles.</p>
  </div>
</section>


<section id="skills">
  <h2>Skills</h2>
  <ul>
    <li><strong>R</strong></li>
    <li><strong>Quarto</strong></li>
    <li><strong>Spreadsheet</strong></li>
    <li><strong>Shiny</strong></li>
    <li><strong>Tableau</strong>: <a href="https://public.tableau.com/app/profile/jiaxun.zou/vizzes" target="_blank">Tableau Public Profile</a></li>
    <li><strong>SAS</strong></li>
    <li><strong>Python</strong></li>
    <li><strong>EViews</strong></li>
  </ul>
</section>

<section id="community">
  <h2>Community</h2>
  <p>Visit my community website: <a href="https://lizicup.netlify.app/" target="_blank">lizicup.netlify.app</a></p>
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
    <li><a href="#community" class="sidebar-link">Community</a></li>
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

    window.addEventListener("scroll", highlightCurrentSection);
  });
</script>