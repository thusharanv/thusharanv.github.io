<style>
  /* Flexbox container to align left and right sections */
  .container {
    display: flex;
    justify-content: space-between;
    gap: 20px; /* Adds space between the left and right sections */
    padding: 20px;
  }

  /* Left section with image and about me */
  .left-side {
    flex: 0 0 40%; /* Occupies 40% of the width */
    padding-right: 20px;
  }

  
  /* Right section with skills and contact */
  .right-side {
    flex: 0 0 55%; /* Occupies 55% of the width */
    max-height: 600px; /* Set a max height for the right pane */
    overflow-y: auto; /* Enable vertical scrolling when content overflows */
    scrollbar-width: none; /* Firefox */
    padding-left: 20px;
  }
  /* Remove scrollbar in Webkit-based browsers (Chrome, Safari) */
  .right-side::-webkit-scrollbar {
    display: none;
  }

  /* Profile image style */
  .profile-image {
    width: 100%; /* Makes image responsive */
    border-radius: 50%; /* Rounds the image */
    margin-bottom: 20px;
    object-fit: cover; /* Ensures image fits well within the circle */
  }
  /* Left section with image, about me, and links */
.left-side {
  flex: 0 0 40%; /* Adjusts width of left section */
  padding-right: 20px; /* Adds some padding to the right */
  text-align: left; /* Center aligns all content in left-side */
}

  /* Heading styles */
  h3 {
    font-size: 1.6em;
    margin-top: 0;
    color: #0d3b66;
  }

  /* Style for paragraphs and lists */
  p, ul {
    font-size: 1em;
    line-height: 1.6;
    
  }
  p, ul, li,h4{
          color: #7285A5; /* Change all paragraphs to blue */
          }

  ul {
    list-style-type: none; /* Removes bullets */
    padding-left: 0;
  }

  ul li {
    margin-bottom: 10px;
  }
 /* Styling for links */
  a {
    color: #0066cc; /* Set the link color to blue or any color of your choice */
    text-decoration: none; /* Remove underline */
  }

  /* Change link color on hover */
  a:hover {
    color: #86C5D8; /* Change to orange or any color you want when the user hovers over the link */
    text-decoration: underline; /* Optional: Adds underline on hover */
  }
  /* Responsive adjustments for smaller screens */
  @media (max-width: 768px) {
    .container {
      flex-direction: column; /* Stack left and right sections vertically on smaller screens */
    }
    .left-side, .right-side {
      flex: 0 0 100%; /* Ensure both sections take full width on smaller screens */
      padding-right: 0;
      padding-left: 0;
    }
  }
</style>

<!-- Main container for left and right columns -->
<div class="container">
  <!-- Left side with image and details -->
  <div class="left-side">
    <img src="asset/images/Untitled.png" alt="Your Image" class="profile-image">
    <!-- Contact Links (GitHub, Resume, LinkedIn, Email) -->
      <div class="contact-links">
      <a href="https://github.com/thusharanv" target="_blank">GitHub</a> |
      <a href="https://www.linkedin.com/in/thushara-namath-vadakkemadathil-606a93187" target="_blank">LinkedIn</a> |
      <a href="https://example.com/your-resume.pdf" target="_blank">Resume</a> |
      <a href="mailto:tnv@udel.edu">Email</a>
      </div>
    <h3>About Me</h3>
    <p>
      Enthusiastic and detail-oriented Data Science graduate | Strong foundation in programming, database management, and data analysis | Passionate about transforming complex datasets into actionable insights | Proficient in Python, SQL, and R 
    </p>
  </div>
  
  <!-- Right side with skills and contact information -->
  <div class="right-side">
    <!-- Education Section under About Me -->
    <h3>Education</h3>
    <ul>
    <li><strong>University of Delaware</strong>, DE, USA</li>
    <li>M.S in Data Science - Feb 2022 – Dec 2024 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<strong>GPA: 4.0</strong> </li>
    <li><strong>Chinmaya Institute of Technology</strong>, Kannur University, India</li>
    <li>Master of Computer Applications - Aug 2008 – Nov 2011</li>
    </ul>  
    <h3>Skills & Expertise</h3>
    <ul>
      <li><strong>Programming Languages:</strong> Python, R, SQL, C, C++</li>
      <li><strong>Data Analysis & Visualization:</strong> Pandas, Matplotlib, Seaborn</li>
      <li><strong>Machine Learning:</strong> Scikit-learn, TensorFlow</li>
      <li><strong>Database Management:</strong> PostgreSQL, MySQL</li>
    </ul>
    <h3>Academic Projects</h3>

<!-- Australia Next Day Rain Prediction -->
<div class="project-item">
  <h4>Australia Next Day Rain Prediction</h4>
  <p><strong>Tools Used:</strong> Python, Random Forest, Logistic Regression, SMOTE, Pandas, Matplotlib</p>
  <p>Developed machine learning models to predict next day rainfall using data from Australia. Applied techniques like feature selection and data balancing to improve model performance. Achieved an accuracy of 85% with Random Forest.</p>
  <p><strong>GitHub Repository:</strong> <a href="https://github.com/your-project-link" target="_blank">View Code</a></p>
</div>

<!-- Stroke Prediction Using Machine Learning -->
<div class="project-item">
  <h4>Stroke Prediction Using Machine Learning</h4>
  <p><strong>Tools Used:</strong> Python, Random Forest, Logistic Regression, PCA, Imbalanced Data Techniques</p>
  <p>Implemented machine learning algorithms to predict the likelihood of a stroke based on a variety of health metrics. Used techniques such as Principal Component Analysis (PCA) for dimensionality reduction and employed Random Forest as the final model.</p>
  <p><strong>GitHub Repository:</strong> <a href="https://github.com/your-project-link" target="_blank">View Code</a></p>
</div>

<!-- Cart Abandonment Prediction -->
<div class="project-item">
  <h4>Cart Abandonment Prediction for E-commerce</h4>
  <p><strong>Tools Used:</strong> Python, Naive Bayes, Decision Trees, Pandas, Scikit-learn</p>
  <p>Analyzed customer behavior data to predict cart abandonment and identify factors influencing purchase decisions. Applied machine learning models to make predictions and suggest solutions for reducing abandonment.</p>
  <p><strong>GitHub Repository:</strong> <a href="https://github.com/your-project-link" target="_blank">View Code</a></p>
</div>
  </div>
</div>
