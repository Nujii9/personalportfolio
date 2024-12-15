<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rubio's Personal Website</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: #5b0400;
            color: #ededed;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .password-container {
            text-align: center;
            background: #2b2b2b;
            padding: 20px 40px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        }

        .password-container h1 {
            font-size: 24px;
            margin-bottom: 20px;
        }

        .password-container input {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
        }

        .password-container button {
            padding: 10px 20px;
            background: #5fdcff;
            border: none;
            border-radius: 5px;
            color: #2b2b2b;
            font-weight: bold;
            cursor: pointer;
            font-size: 16px;
        }

        .password-container button:hover {
            background: #ff347b;
        }

        .error {
            color: #ff347b;
            font-size: 14px;
            margin-top: 10px;
        }
    </style>
</head>

<body>
    <div class="password-container">
        <h1>Before you proceed, please enter password.</h1>
        <input type="password" id="password" placeholder="rubio2024">
        <button onclick="checkPassword()">Submit</button>
        <p id="error" class="error"></p>
    </div>

    <script>
        function checkPassword() {
            const password = document.getElementById('password').value;
            const error = document.getElementById('error');
            const correctPassword = "rubio2024"; 

            if (password === correctPassword) {
                error.textContent = ""; 
                window.location.assign("https://sites.google.com/view/rubio-portfolio/home  "); 
            } else {
                error.textContent = "Incorrect password. Please try again.";
            }
        }
    </script>
</body>

</html>
