<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>InstaLoader</title>
    <!-- ... (existing head content) ... -->
    <script>
        function changeLanguage() {
            var languageSelect = document.getElementById("languageSelect");
            var selectedLanguage = languageSelect.value;
            alert("Selected Language: " + selectedLanguage);
            // You can add logic here to change the language as needed
        }

        function submitForm(event) {
            event.preventDefault();
            var urlInput = document.getElementById("url");
            var resultDiv = document.getElementById("result");

            // You can add logic here to handle the form submission
            var url = urlInput.value;
            resultDiv.innerHTML = "Downloading..."; // Placeholder message, you can replace it with actual logic

            // Example: Creating a download link
            var downloadLink = document.createElement("a");
            downloadLink.href = url;
            downloadLink.download = "downloaded_file"; // You can customize the filename here
            document.body.appendChild(downloadLink);
            downloadLink.click();
            document.body.removeChild(downloadLink);

            resultDiv.innerHTML = "Download successful!";
        }
    </script>

    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }

        h2.sat {
            color: rgb(77, 8, 112);
            text-align: center;
            margin: 10px 0;
        }

        #languageSelect {
            margin-bottom: 20px;
        }

        .menu {
            background-color: plum;
            color: white;
            padding: 20px;
            margin: 20px auto;
            width: 80%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        #enter {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            font-size: 30px;
        }

        .baard {
            text-align: center;
        }

        .head {
            color: rgb(88, 20, 122);
        }

        .baar {
            color: #333;
        }

        section {
            text-align: center;
        }

        #urlForm {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 10px;
            color: rgb(88, 20, 122);
        }

        input {
            width: 80%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        button {
            padding: 10px 20px;
            background-color: rgb(88, 20, 122);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: rgb(68, 10, 102);
        }

        #result {
            font-weight: bold;
            color: rgb(88, 20, 122);
            margin-bottom: 20px;
        }
        .menu a i {
            margin-right: 5px;
        }
    </style>

</head>
<body>
    <h2 class="sat">InstaLoader</h2>
    <select id="languageSelect" onchange="changeLanguage()">
        <option value="en">English</option>
        <option value="fr">French</option>
        <!-- Add more language options as needed -->
    </select>

    <div class="menu">
        <div id="enter">
           <a href="#"><i class="fas fa-video"></i> Video</a>
            <a href="#"><i class="fas fa-image"></i> Image</a>
            <a href="#"><i class="fas fa-book"></i> Story</a>
            <a href="#"><i class="fas fa-users"></i> Real</a>
        </div>

        <h1 class="baard head">
            Instagram Video Download
        </h1>
        <p class="baar">
            Download Video Instagram, Photo, Reels, Stories, IGTV online
        </p>
        <section>
            <form id="urlForm" onsubmit="submitForm(event)">
                <label for="url">Enter URL:</label>
                <input type="url" id="url" name="url" required>
                <button type="submit">Download</button><br>
            </form>
            <div id="result"></div>
        </section>
    </div class="NAV">


    <h1>All features of InstaLoader.App</h1>
    <p>Snapinsta supports all types of Instagram videos/images links</p>
    <img src="https://snapinsta.app/assets/img/thumb/insta-video.webp" alt="" id="harry">
    <img src="https://snapinsta.app/assets/img/thumb/insta-photo.webp" alt="">
    <img src="https://snapinsta.app/assets/img/thumb/insta-reels.webp" alt="">
    <img src="https://snapinsta.app/assets/img/thumb/insta-igtv.webp" alt="">
    </div>
</body>
</html>
# insta
