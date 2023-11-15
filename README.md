# Ex.07 Software Product Company Website
## Date: 24/10/23

## AIM:
To develop a static company website to display the softwares and services provided by the company.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
Mainpage.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant</title>
    <link rel="stylesheet" href="restaurant.css">
</head>
<body>
        <header>
            <h1 style="font-size: 30px;">MJ's Restaurant</h1>
            <nav class="navbar">
                <a href="">Home</a>
                <a href="">Menu</a>
                <a href="">About</a>
            </nav>
        </header>

        <div class="main">
            <div class="about">
            <h1>Welcome to our restaurant</h1>
            <h2>Legendary Foods</h2>
            <p>"The legendary taste of CHENNAI"</p>
            <button>Order us</button>
        </div>
    </div>


    <h1>Foods in our Restaurant</h1>

    <div class="menu">

        <div class="starters">
        <table>
            <th colspan="2">Starters</th>
            <tr>
                <td>Tomato Soup</td>
                <td>&#8377 100</td>           

                </tr>
           <tr>
                <td>Cool drinks</td>
                <td>&#8377 50/each</td>
            </tr>
            <tr>
                <td>Knorr Soup</td>
                <td>&#8377 100</td>
            </tr>
            <tr>
                <td>Veg soup</td>
                <td>&#8377 100</td>
            </tr>
            <tr>
                <td>Chicken Soup</td>
                <td>&#8377 100</td>
            </tr>
        </table>
    </div>
    <div class="food">
        <table>
            <th colspan="2">Items</th>
            <tr>
                <td>Biriyani</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>fried rice</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>fried noodles</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>noodles</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>sea foods</td>
                <td>&#8377 200</td>
            </tr>
        </table>
    </div>

    <div class="chats">
        <table>
            <th colspan="2">Chats</th>
            <tr>
                <td>Biriyani</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>fried rice</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>fried noodles</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>noodles</td>
                <td>&#8377 200</td>
            </tr>
            <tr>
                <td>sea foods</td>
                <td>&#8377 200</td>
            </tr>
        </table>
    </div>
    </div>

    <div class="locations">
        <div class="location1">
            <h1>Anna nagar</h1>
            <address>Anna nagar , kora food street - 123456</address>
            <h2> Contact : 23456789</h2>
        </div>

        <div class="location2">
            <h1>Velachery</h1>
            <address>Velachery , Phoenix mall - 123456</address>
            <h2> Contact : 23456789</h2>
        </div>

        <div class="location3">
            <h1>Porur</h1>
            <address>Vigneshwara nagar, Porur- 123456</address>
            <h2> Contact : 23456789</h2>
        </div>



    </div>

    <section id="photos">
        <div class="photobanner">
            <img src="mithun bg.jpg" alt="">
            <h1>MithunRaj</h1>

            <img src="jose bg.jpg" alt="">
            <h1>Jerushlin Jose</h1>

        </div>
    </section>
            

    
</body>
</html>


```

restaurant.css
```
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins',sans-serif;
}
body{
    background-color: grey;
    height: 100vh;
    width: 100%;
}
header{
    display: flex;
    justify-content: space-between;
    padding-top: 30px;
    background-color: black;
}

header h1{
    color: white;
    font-size: 20px;
    padding-left: 20px;
}
.navbar a{
    margin-right: 15px;
    text-decoration: none;
    color:  black;
    background-color: yellow;
    border-radius: 3px;
    padding: 5px 8px;
}
 .navbar a:hover{
    background-color: white;
    box-shadow: 0 0 10px yellow;
 }

.main{
    display: flex;
    width: 50%;
    margin: 60px;
}
.about{
    display: flex;
    flex-direction: column;
}
.about h1{
    font-size: 40px;
    color: #663399;
    margin-bottom: 20px;

}
.about h2{
    font-size: 30px;
}
.about p{
    margin-top: 10px;
    margin-bottom: 10px;
}
.about button{
    margin-top: 30px;
    width: 40%;
    padding: 10px;
    font-weight: bold;
    border-radius: 8px;
    color: #000000;
    background-color: yellow;
    border: none;
}
.about button:hover{
    background-color: white;
    transition: .3s;
    box-shadow: 0 0 10px black;
}

.menu{
    display: grid;
    grid-template-columns: repeat(auto-fir,minmax(300px,1fr 1fr 1fr));
}

.menu table{
    background-color: blueviolet;
    border: 3px solid black;
    width: 100%;
    padding: 40px;
}

.menu table tr{
    display: flex;
    justify-content: center;
    margin: 20px;
}
.menu table th{
    font-size: 30px;
    color: navy;
}
.menu td:nth-child(1){
    flex: 1;
    justify-self: left;
}

.menu td:nth-child(2){
    justify-self: right;
}

h1{
    font-size: 40px;
    display: flex;
    justify-content: center;
    margin-bottom: 30px;
}

.locations{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: black;
    color: yellow;
}

.locations .location1{
    margin-top: 20px;
    margin-bottom: 30px;
    border: 2px solid black;
}

.locations .location2{
    margin-bottom: 20px;
    border: 2px solid black;
}
.locations .location3{
    border: 2px solid black;
}

#photos .photobanner img {


height: 200px;
width: 200px;
margin-right: 50px;
margin-left: 650px;
background-color: gray;
margin-top: 50px;
}

#photos .photobanner h1 {

    color: black;
    font-size: 20px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
```

## OUTPUT:
![image](https://github.com/Mithunlavanyaraj/softweb/assets/120077786/faec67ff-ed17-4795-8541-8985be98b62d)
![image](https://github.com/Mithunlavanyaraj/softweb/assets/120077786/0abd02c6-3aac-4f44-8648-7440faee75dd)
![image](https://github.com/Mithunlavanyaraj/softweb/assets/120077786/5d2513db-3db0-4bb9-8fde-6ff7b929b3b5)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
