<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>چک لیست تعاملی</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            direction: rtl;
            text-align: center;
        }
        .checklist {
            list-style: none;
            padding: 0;
        }
        .checklist li {
            margin: 10px 0;
            cursor: pointer;
            padding: 10px;
            background-color: #f0f0f0;
            border: 1px solid #ddd;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }
        .checklist li:hover {
            background-color: #d0d0d0;
        }
        #message {
            margin-top: 20px;
            font-size: 18px;
            color: #333;
            line-height: 1.5;
        }
    </style>
</head>
<body>
    <h1>چک لیست تعاملی</h1>
    <ul class="checklist">
        <li onclick="showMessage('متن مربوط به پزشکی')">پزشکی</li>
        <li onclick="showMessage('متن مربوط به اعزام')">اعزام</li>
        <li onclick="showMessage('متن مربوط به معافیت کفالت')">معافیت کفالت</li>
        <li onclick="showMessage('متن مربوط به معافیت شرایط خاص')">معافیت شرایط خاص</li>
        <li onclick="showMessage('متن مربوط به معافیت تحصیلی (دانشجویی و دانش‌آموزی)')">معافیت تحصیلی</li>
    </ul>
    <div id="message"></div>

    <script>
        function showMessage(message) {
            const messageBox = document.getElementById('message');
            messageBox.textContent = message;
        }
    </script>
</body>
</html> 
