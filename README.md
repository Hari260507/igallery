# Ex.08 Design of Interactive Image Gallery
## Date:18.12.24

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

```
ig.html

<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>INTERACTIVE IMAGE GALLERY</title>
    <style>
     *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

body {
    font-family: Arial, sans-serif;
    background-color: #baadad;
    color: #473434;
}

header {
    background-color: #1b1111;
    color: #c0b0b0;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
    gap: 20px;
}

nav a {
    color: #ede0e0;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #99d71c; 
}

main {
    padding: 40px;
    text-align: center;
}

h2 {
    font-size: 5rem;
    margin-bottom: 200px;
    color: #160d0d;
}


.team {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 100px;
    justify-items: center;
    margin-top: 200px;
}



.member img {
    width: 100%;
    height: auto;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 4px solid #090607; 
}

.member h3 {
    font-size: 3rem;
    margin-bottom: 10px;
    color: #151313;
}

.member p {
    font-size: 1.1rem;
    color: #080808;
}

.member:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(210, 195, 195, 0.15);
}

h3 {
    margin-bottom: 10px;
    font-size: 1.5rem;
    color: #d7caca;
}

footer {
    background-color: #6a2424;
    color: #fff;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>
</head>

    <main>
        <h2>INTERACTIVE IMAGE GALLERY </h2>
        <div class="team">
            <div class="member">
                <img src="image1.png" alt="image 1">
                <h3>cherry blossom</h3>
                
            </div>
            <div class="member">
                <img src="image2.png" alt="image2">
                <h3>Eiffel tower<h3>
                
            </div>
            <div class="member">
                <img src="image3.png" alt="image3">
                <h3>Grand piano<h3>
                
            </div>
            
        
    </main>
    <footer><p>&copy; Designed and Developed by Charithrakshi K</p></footer>
</body>
</html>

index.js

const imageDiv = document.getElementById("image");
const originalImageUrl = "";
const originalText = "Hover over an image below to display here.";

function upDate(previewPic) {
  imageDiv.style.backgroundImage = url('${previewPic.src}');
  imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
  imageDiv.style.backgroundImage = url('${originalImageUrl}');
  imageDiv.innerHTML = originalText;
}

```

## OUTPUT:

![alt text]({857DAE47-9159-4446-A0A4-4C21B401EA61}.png)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
