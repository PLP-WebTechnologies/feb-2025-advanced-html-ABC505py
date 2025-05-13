# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

Answer:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Responsive Flexbox Layout</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Navigation Bar -->
  <nav class="navbar">
    <div class="logo">MySite</div>
    <ul class="nav-links">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <div class="container">
    <aside class="sidebar">
      <h2>Sidebar</h2>
      <p>Useful links or information here.</p>
    </aside>

    <main class="main-content">
      <h1>Welcome to My Website</h1>
      <p>This is a responsive page using Flexbox and media queries.</p>
    </main>
  </div>

  <!-- Footer -->
  <footer class="footer">
    <p>&copy; 2025 MySite. All rights reserved.</p>
  </footer>

</body>
</html>

/* Global Styles */
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: white;
}

/* Navigation Bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  padding: 15px 30px;
  color: white;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 20px;
}

/* Container with Sidebar and Main Content */
.container {
  display: flex;
  flex-direction: row;
  padding: 20px;
}

/* Sidebar */
.sidebar {
  flex: 1;
  background-color: #f4f4f4;
  padding: 15px;
  margin-right: 20px;
}

/* Main Content */
.main-content {
  flex: 3;
  background-color: #e9ecef;
  padding: 15px;
}

/* Footer */
.footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 15px;
}

/* Responsive Layout: Tablet */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }

  .sidebar {
    margin-right: 0;
    margin-bottom: 20px;
  }
}

/* Responsive Layout: Mobile */
@media (max-width: 480px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav-links {
    flex-direction: column;
    gap: 10px;
    padding-top: 10px;
  }
}

