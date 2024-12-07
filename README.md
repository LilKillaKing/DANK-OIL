<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DANKIE Store</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .form-container, .payment-options {
            max-width: 400px;
            margin: 0 auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        button {
            padding: 10px 15px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button: hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>Welcome to DANKIE</h1>
    <div class="form-container">
        <h2>Enter Delivery Details</h2>
        <form action="/submit-address" method="POST">
            <label for="name">Full Name:</label><br>
            <input type="text" id="name" name="name" required><br><br>
            <label for="address">Address:</label><br>
            <input type="text" id="address" name="address" required><br><br>
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" required><br><br>
            <button type="submit">Continue to Payment</button>
        </form>
    </div>
    <div class="payment-options">
        <h2>Payment Options</h2>
        <p>Pay with:</p>
        <button onclick="window.location.href='https://cash.app/$yourcashapp'">CashApp</button>
        <button onclick="window.location.href='https://venmo.com/yourvenmo'">Venmo</button>
        <button onclick="window.location.href='https://paypal.me/yourpaypal'">PayPal</button>
        <p>For cryptocurrency, please scan the QR code below:</p>
        <img src="your-crypto-qr-code.png" alt="Crypto QR Code" style="width: 200px;">
    </div>
</body>
</html>
