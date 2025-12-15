<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Search Opinion Box</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f2f2f2;
            padding: 40px;
        }
        h2 {
            text-align: center;
        }
        form {
            text-align: center;
            margin-bottom: 30px;
        }
        input {
            width: 300px;
            padding: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px 15px;
            font-size: 16px;
            margin-left: 5px;
            cursor: pointer;
        }
        table {
            width: 60%;
            margin: auto;
            border-collapse: collapse;
            background: white;
        }
        th, td {
            border: 1px solid #ccc;
            padding: 10px;
            text-align: center;
        }
        th {
            background: #007BFF;
            color: white;
        }
    </style>
</head>
<body>

<h2>User Search Opinion</h2>

<!-- FORM -->
<form id="searchForm" action="https://getform.io/f/bxovoeya" method="POST">
    <input type="text" name="search_opinion" id="searchInput" placeholder="Enter your search opinion" required>
    <button type="submit">Submit</button>
</form>

<!-- TABLE -->
<table>
    <thead>
        <tr>
            <th>S.No</th>
            <th>Search Opinion</th>
        </tr>
    </thead>
    <tbody id="tableBody">
    </tbody>
</table>

<script>
    let count = 1;

    document.getElementById("searchForm").addEventListener("submit", function () {
        const input = document.getElementById("searchInput").value;

        const table = document.getElementById("tableBody");
        const row = table.insertRow();

        row.insertCell(0).innerText = count++;
        row.insertCell(1).innerText = input;
    });
</script>

</body>
</html>

</html>
