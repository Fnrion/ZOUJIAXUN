<!-- Include Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap" rel="stylesheet">

<h1 style="font-family: 'Zou Jiaxun (邹佳迅)', sans-serif; font-size: 36px;">Songti TC</h1>

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

<div class="container">
  <!-- Main Content Section -->
  <div class="main-content">
    <section id="experience">
      <h2>Experience</h2>
      <h3>J.P. Morgan – China (Remote Part-time)</h3>
      <p><em>Assistant Analyst | Sep 2023 - Nov 2023</em></p>
      <ul>
        <li>Collected financial data during the federal rate hike cycle to consolidate data in the database.</li>
        <li>Reviewed and collated data on companies by researching annual reports, IPO letters, and other sources.</li>
        <li>Conducted company research on East Money Credit Co., Ltd., analyzing future market share and profitability.</li>
        <li>Analyzed different index trends and stock valuations (A-share and H-share), providing investment recommendations to the fund manager.</li>
      </ul>

      <h3>Changzhou Jinbaihe – Jiangsu, China</h3>
      <p><em>Account Assistant | Jun 2022 - Aug 2022</em></p>
      <ul>
        <li>Recorded daily transactions in the financial system and checked daily bills to eliminate reporting errors.</li>
        <li>Wrote weekly memos and coordinated with department managers to monitor finances.</li>
        <li>Analyzed financial statements, providing insights on abnormal data like high receivables, and helped increase cash flow by 12%.</li>
      </ul>

      <h3>Gaierpu International Trading Corporation – Jiangsu, China</h3>
      <p><em>Export Trader | Jun 2021 - Aug 2021</em></p>
      <ul>
        <li>Collaborated with a team of three to conduct inventory checks and engaged directly with customers.</li>
        <li>Secured a bulk order of 10,000 N95 masks by connecting with suppliers and negotiating favorable terms.</li>
        <li>Monitored fulfillment, achieving 100% on-time delivery and enhancing customer satisfaction.</li>
      </ul>
    </section>

    <section id="academic-projects">
      <h2>Academic Projects</h2>
      <h3>Illegal Fish Company Business Activity Analysis (R)</h3>
      <p>Developed an interactive visual analytics tool using Shiny to analyze corporate networks of fishery companies potentially involved in illegal, unreported, and unregulated (IUU) fishing activities.</p>
      <ul>
        <li>Processed a knowledge graph with data on companies, owners, employees, and financial status, suitable for network analysis.</li>
        <li>Utilized Centrality Analysis to detect influential entities within the network, identifying ownership structures and control links.</li>
      </ul>

      <h3>IBM Employee Estimated Value Analysis (Python)</h3>
      <p>Built a model to optimize IBM's Employee Estimated Value (EEV) by identifying high-impact factors on employee satisfaction.</p>
      <ul>
        <li>Implemented a Random Forest classifier to identify “at-risk” employees based on job role, performance score, and satisfaction.</li>
        <li>Segmented employees using K-means clustering, enabling targeted interventions for different employee profiles.</li>
        <li>Created Tableau dashboards to visualize employee segments and recommended strategies for each cluster.</li>
      </ul>
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

    <ul style="list-style: none; padding: 0; text-align: center;">
      <li><a href="#about" class="sidebar-link">About</a></li>
      <li><a href="#experience" class="sidebar-link">Experience</a></li>
      <li><a href="#academic-projects" class="sidebar-link">Academic Projects</a></li>
      <li><a href="#contact" class="sidebar-link">Contact</a></li>
    </ul>

    <h3>Additional Skills</h3>
    <p><strong>Technical Skills:</strong> R, Quarto, Spreadsheet, Shiny, Tableau, GPT, SAS, Python, EViews</p>
    <p><strong>Language Skills:</strong> English, Mandarin, French (beginner)</p>
    <p><strong>Work Authorization:</strong> Singapore (Internship), China (Citizen)</p>
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