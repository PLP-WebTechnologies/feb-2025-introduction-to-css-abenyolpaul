# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.



css
/* Reset some default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body styles */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f5f5f5;
    padding: 20px;
}

/* Header styles with ID selector */
#main-header {
    background-color: #2c3e50;
    color: #ecf0f1;
    padding: 20px;
    margin-bottom: 30px;
    border-bottom: 5px solid #e74c3c;
    text-align: center;
}

/* Navigation styles with class selector */
.nav-menu {
    background-color: #34495e;
    padding: 10px;
    margin-bottom: 20px;
    border-radius: 5px;
}

.nav-menu ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
}

.nav-menu li {
    margin: 0 15px;
}

.nav-menu a {
    color: #ecf0f1;
    text-decoration: none;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 3px;
    transition: background-color 0.3s;
}

.nav-menu a:hover {
    background-color: #e74c3c;
}

/* Main content area */
.main-content {
    background-color: white;
    padding: 25px;
    margin-bottom: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

/* Article styles with class selector */
.article {
    margin-bottom: 30px;
    padding-bottom: 20px;
    border-bottom: 1px dashed #bdc3c7;
}

.article:last-child {
    border-bottom: none;
}

.article h2 {
    color: #2c3e50;
    margin-bottom: 15px;
    font-family: 'Georgia', serif;
}

.article p {
    margin-bottom: 15px;
}

/* Button styles with class selector */
.btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: #3498db;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    border: none;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
}

.btn:hover {
    background-color: #2980b9;
}

/* Special button variation */
.btn-danger {
    background-color: #e74c3c;
}

.btn-danger:hover {
    background-color: #c0392b;
}

/* Sidebar styles with ID selector */
#sidebar {
    background-color: #ecf0f1;
    padding: 20px;
    border: 1px solid #bdc3c7;
    border-radius: 5px;
}

#sidebar h3 {
    color: #2c3e50;
    margin-bottom: 15px;
    font-size: 1.3em;
}

/* Footer styles */
#main-footer {
    background-color: #2c3e50;
    color: #ecf0f1;
    text-align: center;
    padding: 15px;
    margin-top: 30px;
    border-top: 5px solid #e74c3c;
}

/* Utility classes */
.text-center {
    text-align: center;
}

.text-primary {
    color: #3498db;
}

.mt-20 {
    margin-top: 20px;
}

.mb-20 {
    margin-bottom: 20px;
}

.p-10 {
    padding: 10px;
}

.rounded {
    border-radius: 5px;
}

/* Responsive layout */
@media (min-width: 768px) {
    .container {
        display: flex;
        gap: 20px;
    }
    
    .main-content {
        flex: 2;
    }
    
    #sidebar {
        flex: 1;
    }
}
Corresponding HTML Structure
To use this CSS, here's a basic HTML structure you could apply it to:

html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header id="main-header">
        <h1>My Website</h1>
    </header>

    <nav class="nav-menu">
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <main class="main-content">
            <article class="article">
                <h2>Article Title</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris.</p>
                <a href="#" class="btn">Read More</a>
            </article>

            <article class="article">
                <h2>Another Article</h2>
                <p>Vivamus luctus urna sed urna ultricies ac tempor dui sagittis.</p>
                <a href="#" class="btn btn-danger">Warning</a>
            </article>
        </main>

        <aside id="sidebar">
            <h3>Sidebar</h3>
            <p>Some sidebar content here.</p>
            <p class="text-primary">Highlighted text.</p>
        </aside>
    </div>

    <footer id="main-footer">
        <p>&copy; 2023 My Website. All rights reserved.</p>
    </footer>
</body>
</html>
This CSS demonstrates:

Class selectors (.nav-menu, .article, .btn)

ID selectors (#main-header, #sidebar, #main-footer)

Color properties (background-color, color)

Typography (font-family, font-size, line-height)

Margins and paddings (margin, padding)

Borders (border, border-radius)

Responsive design with media queries

Utility classes for common styling needs

Hover effects and transitions

New chat
Message DeepSeek
AI-generated, for reference only


>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨
