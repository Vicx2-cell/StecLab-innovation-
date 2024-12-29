<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StecLab Innovations</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: black;
            color: white;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #003366;
            text-align: center;
            padding: 50px 0;
        }

        header h1 {
            font-size: 2.5em;
            margin: 0;
        }

        header p {
            font-size: 1.2em;
        }

        .container {
            padding: 20px;
            max-width: 600px;
            margin: 0 auto;
        }

        form {
            background-color: #1a1a1a;
            padding: 30px;
            border-radius: 8px;
        }

        label {
            display: block;
            margin-bottom: 10px;
            font-size: 1.2em;
        }

        input[type="text"], input[type="email"], select, button {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 2px solid #003366;
            border-radius: 4px;
            font-size: 1.1em;
        }

        input[type="radio"] {
            margin-right: 10px;
        }

        button {
            background-color: #003366;
            color: white;
            border: none;
            font-size: 1.2em;
            cursor: pointer;
        }

        button:hover {
            background-color: #00509e;
        }

        .whatsapp-prompt {
            margin-top: 20px;
            font-size: 1.1em;
        }

        .message {
            text-align: center;
            font-size: 1.2em;
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
        <p>Owned by Chibuike Iheanyichi Victor - Born 10 February 2008</p>
        <p>Vision: To Grow Digital Life with AI</p>
    </header>

    <div class="container">
        <h2>Register for a Course</h2>
        <form id="registrationForm">
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Your Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="course">Choose Course:</label>
            <select id="course" name="course" required>
                <option value="virtual_assistance">Virtual Assistance</option>
                <option value="data_analysis">Data Analysis</option>
                <option value="web_development">Web Development with AI</option>
            </select>

            <label>Would you like to join our WhatsApp group?</label>
            <input type="radio" id="joinYes" name="joinWhatsapp" value="yes" required> Yes
            <input type="radio" id="joinNo" name="joinWhatsapp" value="no"> No

            <button type="submit">Submit</button>
        </form>

        <div id="message" class="message"></div>
    </div>

    <script>
        document.getElementById("registrationForm").addEventListener("submit", function (event) {
            event.preventDefault(); // Prevent form submission

            // Get form values
            const name = document.getElementById("name").value;
            const email = document.getElementById("email").value;
            const course = document.getElementById("course").value;
            const joinWhatsapp = document.querySelector('input[name="joinWhatsapp"]:checked').value;

            // Show message on form submission
            const messageDiv = document.getElementById("message");

            // Handle WhatsApp redirection based on user's choice
            if (joinWhatsapp === "yes") {
                messageDiv.innerHTML = `<p>Thank you, ${name}. You will be redirected to the WhatsApp group.</p>`;
                setTimeout(function () {
                    window.location.href = "https://chat.whatsapp.com/CHEWG7CAUn24T5VJpg4m7G"; // Redirect to WhatsApp group
                }, 2000); // Redirect after 2 seconds
            } else {
                messageDiv.innerHTML = `<p>Thank you, ${name}. You will not be redirected to the WhatsApp group.</p>`;
            }

            // Simulate sending email notification (for the sake of the example, real backend needed for actual email)
            console.log(`Email sent to: chibuikevictor692@gmail.com`);
            console.log(`Form details: Name: ${name}, Email: ${email}, Course: ${course}`);
        });
    </script>
</body>

</html>
