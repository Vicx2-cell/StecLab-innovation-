<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StecLab Innovations</title>
    <style>
        /* General Styling */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f9;
            color: #333;
        }

        /* Header Styling */
        header {
            background: linear-gradient(90deg, #003366, #00509e);
            color: white;
            text-align: center;
            padding: 30px 20px;
        }

        header h1 {
            font-size: 3rem;
            margin: 0;
        }

        header p {
            font-size: 1.2rem;
            margin-top: 10px;
        }

        /* Navigation Bar */
        nav {
            background-color: white;
            box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
        }

        nav ul li {
          margin: 0 19px; 
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
            font-size: 1.1rem;
        }

        nav ul li a:hover {
            color: #00509e;
        }

        /* Section Styling */
        section {
            padding: 50px 20px;
            text-align: center;
        }

        #about {
            background-color: #f9f9f9;
        }

        #courses {
            background-color: #ffffff;
        }

        #contact {
            background-color: #f9f9f9;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #003366;
        }

        p {
            font-size: 1rem;
            line-height: 1.8;
        }

        /* Form Styling */
        form {
            background-color: #ffffff;
            padding: 30px;
            max-width: 500px;
            margin: 0 auto;
            border-radius: 10px;
            box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
        }

        form label {
            display: block;
            margin: 10px 0 5px;
            font-size: 1.1rem;
        }

        form input[type="text"],
        form input[type="email"],
        form input[type="tel"],
        form select,
        form button {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }

        form input[type="radio"] {
            margin-right: 10px;
        }

        form button {
            background-color: #003366;
            color: white;
            border: none;
            font-size: 1.2rem;
            cursor: pointer;
        }

        form button:hover {
            background-color: #00509e;
        }

        .message {
            text-align: center;
            font-size: 1rem;
            color: green;
            margin-top: 20px;
        }

        .message.error {
            color: red;
        }
    </style>
</head>

<body>
    <header>
        <h1>StecLab Innovations</h1>
        <p>Empowering digital growth through innovation, connection, and transformation.</p>
    </header>

    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#courses">Courses</a></li>
            <li><a href="#register">Register</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="about">
        <h2>About Us</h2>
        <p>StecLab Innovations is a platform designed to empower individuals with the latest in digital technology and skills. From web development to data analysis, we provide tools and resources to make innovation a reality.</p>
    </section>

    <section id="courses">
        <h2>Our Courses</h2>
        <p>We offer a variety of courses to suit your needs:</p>
        <ul>
            <li>Virtual Assistance (Paid)</li>
            <li>Data Analysis (Paid)</li>
            <li>Web Development with AI (Free and Paid)</li>
        </ul>
    </section>

    <section id="register">
        <h2>Register for a Course</h2>
        <form action="https://formspree.io/f/mpwwrkla" method="POST">
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Your Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="course">Choose a Course:</label>
            <select id="course" name="course" required>
                <option value="virtual_assistance">Virtual Assistance (Paid)</option>
                <option value="data_analysis">Data Analysis (Paid)</option>
                <option value="web_development">Web Development with AI (Free and Paid)</option>
            </select>

            <label>Would you like to join our WhatsApp group?</label>
            <input type="radio" id="joinYes" name="joinWhatsapp" value="Yes" required> Yes
            <input type="radio" id="joinNo" name="joinWhatsapp" value="No"> No

            <label for="whatsappNumber">WhatsApp Number:</label>
            <input type="tel" id="whatsappNumber" name="whatsappNumber" placeholder="Enter your WhatsApp number" required>

            <button type="submit">Submit</button>
        </form>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>For sponsorships and inquiries, contact: 08082531673</p>
        <p>Join our WhatsApp group: <a href="https://chat.whatsapp.com/CHEWG7CAUn24T5VJpg4m7G" target="_blank">Click Here</a></p>
    </section>
</body>

</html>