<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eco Smart Waste Management | Login</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', 'Segoe UI', sans-serif;
        }

        body {
            /* Soft eco-friendly gradient */
            background: linear-gradient(135deg, #e8f5e9 0%, #c8e6c9 100%);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #2e7d32;
        }

        .login-card {
            background: #ffffff;
            padding: 45px 35px;
            border-radius: 30px;
            box-shadow: 0 15px 35px rgba(46, 125, 50, 0.1);
            width: 100%;
            max-width: 420px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        /* Eco-Smart Logo Icon */
        .brand-icon {
            background: #4caf50;
            width: 64px;
            height: 64px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 20px;
            box-shadow: 0 8px 20px rgba(76, 175, 80, 0.3);
        }

        h2 {
            font-size: 22px;
            color: #1b5e20;
            margin-bottom: 5px;
            letter-spacing: -0.5px;
        }

        p.subtitle {
            font-size: 14px;
            color: #66bb6a;
            margin-bottom: 30px;
            font-weight: 500;
        }

        /* Input Styling */
        .input-group {
            margin-bottom: 18px;
            text-align: left;
        }

        input {
            width: 100%;
            padding: 15px 20px;
            border: 2px solid #f1f8e9;
            border-radius: 15px;
            background: #f9fbf9;
            font-size: 15px;
            transition: all 0.3s ease;
            outline: none;
            color: #333;
        }

        input:focus {
            border-color: #4caf50;
            background: #fff;
            box-shadow: 0 0 10px rgba(76, 175, 80, 0.1);
        }

        /* Eco Button */
        .login-btn {
            width: 100%;
            padding: 15px;
            background: #2e7d32;
            color: white;
            border: none;
            border-radius: 15px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
        }

        .login-btn:hover {
            background: #1b5e20;
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(27, 94, 32, 0.2);
        }

        /* Results Display */
        #result {
            margin-top: 20px;
            font-size: 14px;
            font-weight: 600;
            min-height: 20px;
        }

        .version-tag {
            margin-top: 25px;
            font-size: 11px;
            color: #a5d6a7;
            text-transform: uppercase;
            letter-spacing: 1.5px;
        }
    </style>
</head>
<body>

    <div class="login-card">
        <div class="brand-icon">
            <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
                <path d="M11 20A7 7 0 0 1 9.8 6.1C15.5 5 17 4.48 19 2c1 2 2 4.18 2 8a8 8 0 0 1-10 10Z"></path>
                <path d="M7 21c-4.3 0-7-3-7-7 0-3 2.5-6 7-6"></path>
                <circle cx="12" cy="12" r="2"></circle>
            </svg>
        </div>

        <h2>Eco Smart Waste</h2>
        <p class="subtitle">Management System</p>

        <input type="text" id="username" placeholder="Officer Username" autocomplete="off">
        <br><br>
        <input type="password" id="password" placeholder="System Password">

        <button class="login-btn" onclick="login()">Sign In to Dashboard</button>

        <p id="result"></p>

        <div class="version-tag">Sustainable Tech • v1.2</div>
    </div>

    <script>
        function login() {
            const user = document.getElementById("username").value;
            const pass = document.getElementById("password").value;
            const resultElement = document.getElementById("result");

            if (user === "admin" && pass === "1234") {
                resultElement.innerText = "Success! Securing connection...";
                resultElement.style.color = "#2e7d32";
                
                // Example: redirecting to the smart bin monitoring page
                // setTimeout(() => { window.location.href = "bins_status.html"; }, 1200);
            } else {
                resultElement.innerText = "Invalid credentials. Access Denied.";
                resultElement.style.color = "#d32f2f";
            }
        }
    </script>
</body>
</html>
