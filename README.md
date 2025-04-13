# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Flexbox Layout</title>
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* Navigation Bar */
    nav {
      background-color: #333;
      padding: 10px;
    }

    nav ul {
      display: flex;
      justify-content: space-around;
      list-style-type: none;
      margin: 0;
      padding: 0;
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 10px;
      display: block;
    }

    /* Main Content */
    main {
      display: flex;
      justify-content: space-around;
      padding: 20px;
    }

    section {
      background-color: #f4f4f4;
      padding: 20px;
      margin: 10px;
      flex: 1;
      min-width: 200px;
    }

    /* Media Queries for Responsiveness */

    /* Tablet View */
    @media (max-width: 768px) {
      nav ul {
        flex-direction: column;
        align-items: center;
      }

      main {
        flex-direction: column;
        align-items: center;
      }
    }

    /* Mobile View */
    @media (max-width: 480px) {
      nav a {
        padding: 8px;
      }

      section {
        padding: 15px;
        margin: 5px;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <main>
    <section>Section 1</section>
    <section>Section 2</section>
    <section>Section 3</section>
  </main>

</body>
</html>
