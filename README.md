<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Search Box</title>
    <style>
        body {
            font-family: Arial;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: #f4f4f4;
        }
        form {
            background: white;
            padding: 20px;
            border-radius: 10px;
        }
        input[type="text"] {
            width: 250px;
            padding: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px 15px;
            font-size: 16px;
            margin-left: 5px;
        }
    </style>
</head>
<body>

<form action="https://formspree.io/f/abcdwxyz" method="POST">
    <input type="text" name="search_input" placeholder="Enter your search" required>
    <button type="submit">Search</button>
</form>

</body>
</html>
