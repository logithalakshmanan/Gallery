# Ex.07 Design of Interactive Image Gallery
# Date:12.12.2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
gallery.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
</head>
<body>
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>ATTACK ON TITAN</h1>
    </header>

    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="aot.jpg" style="height: 300px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="eren.jpg" style="height: 300px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="levi.jpg" style="height: 300px;">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="mikasa.jpg" style="height: 300px;">
        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>
```
# OUTPUT:
![alt text](<Screenshot (173).png>)
![alt text](<Screenshot (174).png>)
![alt text](<Screenshot (175).png>)
![alt text](<Screenshot (176).png>)
![alt text](<Screenshot (177).png>)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
