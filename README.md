# Ex.06 Book Front Cover Page Design
# Date:6-10-2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
```
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Cover with Photos</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color:rgb(116, 209, 16);
            overflow: hidden; 
        }

        .book-cover {
            width: 380px;
            height: 540px;
            position: relative; 
            box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5);
            font-family: 'Georgia', serif;
            text-align: center;
            border-radius: 5px; 
            overflow: hidden; 
        }

        .background-photo {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; 
            filter: brightness(90%) contrast(130%); 
            z-index: 1;
        }

        .author-photo {
            position: absolute; 
            bottom: 10px; 
            left: 50%;
            transform: translateX(-50%); 
            width: 80px; 
            height: 80px;
            border-radius: 50%; 
            border: 3px solid #36a909; 
            object-fit: cover;
            z-index: 3; 
            margin-left: 50px;
            margin-bottom: 85px;
        }

        .cover-content {
            position: relative; 
            z-index: 2; 
            display: flex;
            flex-direction: column;
            justify-content: space-between; 
            height: 100%; 
            padding: 20px;
            box-sizing: border-box; 
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7); 
        }

        .book-title {
            color:  #f91706; 
            font-size: 2.2em;
            font-weight: bold;
            text-transform: uppercase;
            line-height: 1.1;
            margin-top: 30px; 
        }

        .book-subtitle {
            color: #e5f016; 
            font-size: 1.1em;
            margin-top: 10px;
            flex-grow: 1; 
            display: flex;
            align-items: center; 
            justify-content: center;
        }

        .book-author {
            color: #ed2e08; 
            font-size: 1.4em;
            font-style: italic;
            margin-bottom: 30px; 
            margin-left: 30px;
        }
        body{
            background-image: linear-gradient(rgb(250, 69, 69),rgb(29, 237, 209),rgb(230, 230, 27));

        }
    </style>
</head>
<body >
>
    
    <div class="book-cover">
        
        <img src="{% static 'pb.jpg' %}" class="background-photo" height="515" width="330">

        <img src="{% static 'ps.jpg' %}" alt="Author's Photo" class="author-photo">
         
        

        <div class="cover-content">
            <h1 class="book-title">The Legend of Lightning McQueen</h1>
            <h2 class="book-subtitle">Where Speed Meets Heart,Friendship Courage and Victory</h2>
            <p class="book-author">BHUVANESH S</p>
        </div>
    </div>

</body>
</html>
```
# OUTPUT:
![alt text](<Screenshot 2025-10-06 092739.png>)
# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
