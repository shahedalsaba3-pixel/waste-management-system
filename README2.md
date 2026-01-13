<!DOCTYPE html>
<html>
<head>
    <title>Login Page</title>
    <style>
        /* دمج الـ CSS هنا */
        body {
            font-family: Arial;
            text-align: center;
            margin-top: 50px;
        }

        input {
            padding: 5px;
        }

        button {
            padding: 5px 10px;
            cursor: pointer;
        }

        #result {
            margin-top: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h2>Login</h2>

    <input type="text" id="username" placeholder="Username">
    <br><br>
    <input type="password" id="password" placeholder="Password">
    <br><br>

    <button onclick="login()">Login</button>

    <p id="result"></p>

    <script>
        /* دمج الـ JS هنا */
        function login() {
            var user = document.getElementById("username").value;
            var pass = document.getElementById("password").value;

            if (user === "admin" && pass === "1234") {
                document.getElementById("result").innerText = "Login Successful";
                document.getElementById("result").style.color = "green";
            } else {
                document.getElementById("result").innerText = "Login Failed";
                document.getElementById("result").style.color = "red";
            }
        }
    </script>
</body>
</html>
