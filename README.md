<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website</title>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }

        .container {
            background-image: url('./images/1 (1).jpg'); 
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
            color: white;
            max-width: 100%; 
        }

        .main {
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            max-width: 100%;
        }

        .content {
            display: flex;
            align-items: center;
        }

        .content > a {
            margin-left: 20px;
            padding: 10px;
            margin-right: 20px;
            text-decoration: none;
            color: white;
            font-size: 20px;
        }

        .dropdown {
            position: relative;
            display: inline-block;
        }

        .dropdown a {
            color: white; 
            text-decoration: none; 
            font-size: 20px;
        }

        .dropdown-content {
            display: none;
            position: absolute;
            background-color: white;
            min-width: 150px;
            z-index: 1;
            border-radius: 10px;
        }

        .dropdown-content a {
            color: black;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
        }

        .dropdown:hover .dropdown-content {
            display: block;
        }

        .profile-image {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            max-width: 100%;
            margin-bottom: 5px;
        }

        .intro {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 100%;
            max-width: 100%;
            margin-bottom: 150px;
        }

        .welcome-bar-wrapper {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .welcome {
            background-color: white;
            color: black;
            font-size: 20px;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .bar-wrapper {
            display: inline-block;
            margin: 0 10px; 
            text-align: center;
            color: black;
            padding: 30px;
        }

        .bar-parent {
            background-color: black;
            width: 200px;
            border-radius: 20px;
            margin-bottom: 20px;
        }

        .bar-children {
            height: 6px;
            background-color: #22a57c;
            border-radius: 20px;
        }

        .white-bg {
            background-color: white;
        }

        .hire-section {
            background-image: url('./images/3.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: space-around;
            align-items: center;
            padding: 10px;
            color: white;
            max-width: 100%; 
            flex-direction: column;
            position: relative;
        }

        .hire-section-overlay {
            background-color: rgba(0, 0, 0, 0.5);
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
        }

        .hire-section-content {
            background-color: rgba(255, 255, 255, 0.7);
            border-radius: 10px;
            padding: 20px;
            text-align: center;
        }

        .box {
            display: flex;
            justify-content: space-around;
            align-items: center;
            width: 100%;
            max-width: 100%;
            margin-bottom: 5px;
        }

        .hire {
            text-align: center;
        }

        .hire h1 {
            font-size: 24px;
        }

        .hire p {
            font-size: 18px;
        }

        .square-box {
            width: 300px;
            height: 300px;
            border-radius: 30px;
            background-color: transparent;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            transition: background-color 0.3s ease;
            cursor: pointer;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5); 
        }

        .square-box:hover {
            background-color: black;
        }

        .square-box-content {
            color: white;
            font-size: 18px;
        }

        .hobby {
            background-color: white;
            color: black;
            font-size: 20px;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            text-align: center;
            width: 100%;
            max-width: 100%;
            justify-content: center;
        }

        .projects {
            width: 100px;
            height: 40px;
            border-radius: 10px;
            background-color: transparent;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            transition: background-color 0.3s ease;
            cursor: pointer;
            border: 1px solid black; 
            margin-right: 5px; 
            padding: 5px;
            margin-bottom: 10px;
        }
        .box{
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            max-width: 100%;
            margin-bottom: 5px;
        }
        
        .project {
            color: black;
            font-size: 18px;

        }
        
        .projects:hover {
            background-color: green;
            color: white;
        }        

        .pictures {
            display: flex;
            justify-content: space-between;
            margin-left: auto;
            margin: 10px;
        }

        .qualifications {
            background-image: url(./images/man-dslr.jpg);
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            width: 100%;
            height: 100%;
            display: flex;
            padding: 10px;
            color: white;
            max-width: 100%;
            flex-direction: row;
            position: relative;
            margin-right: 10px;
        }

        .experience {
            width: 600px;
            height: 850px;
            background-color: transparent;
            display: flex;
            flex-direction: column;
            transition: background-color 0.3s ease;
            cursor: pointer;
            padding: 50px;
            margin-right: 50px;
        }

        .education{
            width: 600px;
            height: 850px;
            background-color: transparent;
            display: flex;
            flex-direction: column;
            transition: background-color 0.3s ease;
            cursor: pointer;
            padding: 50px;
            margin-right: 50px;
        }

        .small-box{
            width: 100px;
            height: 30px;
            background-color: transparent;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            transition: background-color 0.3s ease;
            cursor: pointer;
            border: 2px solid rgb(5, 149, 82); 
            margin-right: 5px; 
            padding: 5px;
            margin-bottom: 10px;
            font-size: 20px;
        }
        .thin-line{
            border: none;
            border-top: 2px solid #ccc; 
            margin: 20px 0;
        }
        .opinion{
            background-color: white;
            color: black;
            font-size: 20px;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            text-align: center;
            width: 100%;
            max-width: 100%;
            justify-content: center;
        }
        .slider-container {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            overflow: hidden;
            position: relative;
        }

        .slider {
            width: 100%;
            display: flex;
            animation: slide 10s linear infinite; 
        }

        .slide {
            flex: 0 0 100%;
            height: 500px; 
            transition: transform 1s ease;
        }

        .slide img {
            width: 350px;
            height: 350px;
            object-fit: cover;
        }

        @keyframes slide {
            0%, 100% {
                transform: translateX(0);
            }
            20% {
                transform: translateX(0);
            }
            25% {
                transform: translateX(-100%);
            }
            45% {
                transform: translateX(-100%);
            }
            50% {
                transform: translateX(-200%);
            }
            70% {
                transform: translateX(-200%);
            }
            75% {
                transform: translateX(-300%);
            }
            95% {
                transform: translateX(-300%);
            }
            100% {
                transform: translateX(-400%);
            }
        }
        .footer {
            background-color: #333; 
            color: white; 
            text-align: center;
            padding: 20px 0; 
        }

        .social-icons {
            font-size: 24px; 
            margin-right: 10px; 
            color: white;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="main">
            <h1>Apil Adhikari</h1>
            <div class="content">
                <a href="#">Home</a>
                <a href="#">About</a>
                <a href="#">Services</a>
                <div class="dropdown">
                    <a href="#">Pages</a>
                    <div class="dropdown-content">
                        <a href="#">Blog</a>
                        <a href="#">Single Blog</a>
                        <a href="#">Landing page</a>
                    </div>
                </div>
                <a href="#">Contact</a>
            </div>
        </div>
        <div class="profile-image">
            <img src="./images/c1.jpg" alt="profile image" width="150" height="150" style="border-radius: 50%;">
            <h1></h1>
        </div>
        <div class="intro" id="home">
            <h1>My name is <span style="color: red;">KP Oli</span></h1>
            <h2>I am a <span style="color: red;">Web Developer</span></h2>
        </div>
        <div class="welcome-bar-wrapper white-bg">
            <div class="welcome">
                <h1>Welcome to my website</h1>
                <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc, ut rhoncus turpis sodales quis. Integer sit amet mattis quam.Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc</p>
            </div>
            <div class="apil">
            <div class="bar-wrapper">
                <h3>Design</h3>
                <div class="bar-parent">
                    <div class="bar-children"></div>
                </div>
            </div>
            <div class="bar-wrapper">
                <h3>Marketing</h3>
                <div class="bar-parent">
                    <div class="bar-children"></div>
                </div>
            </div>
            <div class="bar-wrapper">
                <h3>Photography</h3>
                <div class="bar-parent">
                    <div class="bar-children"></div>
                </div>
            </div>
            </div>
            <div class="apil">
                <div class="bar-wrapper">
                    <h3>Branding</h3>
                    <div class="bar-parent">
                        <div class="bar-children"></div>
                    </div>
                </div>
                <div class="bar-wrapper">
                    <h3>Softwarica</h3>
                    <div class="bar-parent">
                        <div class="bar-children"></div>
                    </div>
                </div>
                <div class="bar-wrapper">
                    <h3>Pokhara</h3>
                    <div class="bar-parent">
                        <div class="bar-children"></div>
                    </div>
                </div>
                </div>
        </div>
    </div>
    <div class="hire-section">
        <div class="hire">
            <h1>I'm Available For Hire</h1>
            <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc, ut rhoncus turpis sodales quis. Integer sit amet mattis quam.</p>
            <br><br>
        </div>
        <div class="box">
            <div class="square-box">
                <div class="square-box-content">
                    <img src="./images/brush.png">
                    <h2>Design</h2>
                    <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc</p>
                </div>
            </div>
            <div class="square-box">
                <div class="square-box-content">
                    <img src="./images/brush.png">
                    <h2>Marketing</h2>
                    <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc</p>
                </div>
            </div>
            <div class="square-box">
                <div class="square-box-content">
                    <img src="./images/brush.png">
                    <h2>Photography</h2>
                    <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc</p>
                </div>
            </div>
        </div>
    </div>
    <div class="hobby">
        <h1>I love what I do</h1>
        <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc, ut rhoncus turpis sodales quis. Integer sit amet mattis quam.</p>
        <br>
        <br>
        <div class="box">
            <div class="projects" style="margin-right: 50px;">
                Projects
            </div>
            <div class="projects" style="margin-right: 50px;">
                Illustrations
            </div>
            <div class="projects" style="margin-right: 50px;">
                Photography
            </div>
            <div class="projects" style="margin-right: 50px;">
                Website
            </div>
        </div>
        <br>
        <br>
        <div class="pictures1">
            <img src="./images/g1.jpg" height="200px" width="250px" style="margin-right: 50px;">
            <img src="./images/g2.jpg" height="200px" width="250px" style="margin-right: 50px;">
            <img src="./images/g3.jpg" height="200px" width="250px">
            <br><br><br>
        </div>
        <div class="pictures2">
            <img src="./images/g4.jpg" height="200px" width="250px" style="margin-right: 50px;">
            <img src="./images/g5.jpg" height="200px" width="250px" style="margin-right: 50px;">
            <img src="./images/g6.jpg" height="200px" width="250px">
        </div>
    </div>
    <div class="qualifications">
        <div class="experience">
            <h1>Experience</h1>
            <br>
            <br>
            <div class="small-box">2018 - now</div>
            <h3>Full-time Freelancer</h3>
            <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae.</p>
            <hr class="thin-line">
            <br>
            <div class="small-box">2016 - 2018</div>
            <h3>Creative Director at Pixar Studio</h3>
            <p>Accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto.</p>
            <hr class="thin-line">
            <br>
            <div class="small-box">2014 - 2016</div>
            <h3>Senior Designer at Google</h3>
            <p>Accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto.</p>
            <hr class="thin-line">

        </div>
        <div class="education">
            <h1>Education</h1>
            <br>
            <br>
            <div class="small-box">2010</div>
            <h3>Master Degree in Computer Science</h3>
            <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae.</p>
            <hr class="thin-line">
            <br>
            <div class="small-box">2008</div>
            <h3>Bachelor Degree in Computer Science</h3>
            <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae.</p>
            <hr class="thin-line">
            <br>
            <div class="small-box">2004</div>
            <h3>High School Graduation</h3>
            <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae.</p>
            <hr class="thin-line">
        </div>
    </div>
    <div class="opinion">
        <h1>What people say about me</h1>
        <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla mollis dapibus nunc, ut rhoncus turpis sodales quis. Integer sit amet mattis quam.</p>
        <br>
        <div class="slider-container">
            <div class="slider">
                <div class="slide">
                    <img src="./images/aa.png" alt="Slide 1" height="200px" width="200px" >
                </div>
                <div class="slide">
                    <img src="./images/aa - Copy.png" alt="Slide 2" height="200px" width="200px">
                </div>
                <div class="slide">
                    <img src="./images/aa - Copy (2).png" alt="Slide 3" height="200px" width="200px">
                </div>
                <div class="slide">
                    <img src="./images/aa - Copy (3).png" alt="Slide 4" height="200px" width="200px">
                </div>
                <div class="slide">
                    <img src="./images/aa - Copy (4).png" alt="Slide 5" height="200px" width="200px">
                </div>
                <div class="slide">
                    <img src="./images/aa - Copy (5).png" alt="Slide 6" height="200px" width="200px">
                </div>
            </div>
        </div>
    </div>
    <footer class="footer">
        <a href="#" class="social-icons" target="_blank"><i class="fab fa-facebook"></i></a>
        <a href="#" class="social-icons" target="_blank"><i class="fab fa-twitter"></i></a>
        <a href="#" class="social-icons" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="#" class="social-icons" target="_blank"><i class="fab fa-linkedin"></i></a>
        <br>
        <center>
        <hr class="thin-line" width="300px">
        </center>
        <br>
        <p>&copy; 2023 Your Website. All rights reserved.</p>
    </footer>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

</body>
</html>
