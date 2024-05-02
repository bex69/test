<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Image and Text Display</title>
<style>
    body {
        margin: 0;
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: black;
        color: gold; /* Sets text color to gold */
    }
    #container {
        display: flex;
        width: 90%; /* Adjusts the width of the container */
        max-width: 1200px; /* Maximum width of the container */
        height: 80vh; /* Adjusts the height of the container */
    }
    #textSide {
        flex: 1;
        font-size: 24px;
        padding-right: 20px; /* Adds spacing between text and image */
    }
    #imageSide {
        flex: 1;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    img {
        max-width: 100%;
        max-height: 100%;
    }
    #nextButton {
        position: fixed;
        bottom: 20px;
        right: 20px;
        padding: 10px 20px;
        font-size: 16px;
        cursor: pointer;
    }
</style>
</head>
<body>

<div id="container">
    <div id="textSide">
        Here is some text on the left side of the screen. Adjust this text to whatever you need.
    </div>
    <div id="imageSide">
        <img src="yourimage.jpg" alt="Descriptive Alt Text">
    </div>
</div>

<button id="nextButton">Next</button>

<script>
    const nextButton = document.getElementById('nextButton');
    nextButton.onclick = function() {
        window.location.href = 'nextpage.html'; // Replace 'nextpage.html' with your actual next page
    };
</script>

</body>
</html>
