<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Button with Hidden Info and Back Button</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Georgia', serif; /* Using the Georgia serif font */
            font-size: 16px; /* Font size */
            color: #333; /* Text color */
            line-height: 1.6; /* Line spacing */
        }

        .message {
            font-family: 'Times New Roman', serif; /* Change the font to Times New Roman */
            font-size: 18px;
            color: #444; /* Slightly lighter text color */
            margin-top: 20px;
        }

        /* Optional: Add some padding and border around the message */
        .message-box {
            border: 1px solid #ccc;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 5px;
        }
    </style>
    <style>
        /* Button styling */
        .info-button {
            font-size: 2rem;
            background-color: #007BFF;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 5px;
            display: flex;
            align-items: center;
        }

        .info-button i {
            margin-right: 10px;
        }

        /* Hidden information styling */
        .hidden-info {
            display: none;
            margin-top: 20px;
            background-color: #f8f9fa;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        /* Back button styling */
        .back-button {
            font-size: 1.5rem;
            background-color: #eb6d64;
            color: white;
            border: none;
            padding: 8px 16px;
            margin-top: 15px;
            cursor: pointer;
            border-radius: 5px;
        }

        /* Hover effects */
        .info-button:hover {
            background-color: #0056b3;
        }

        .back-button:hover {
            background-color: #db9693;
        }
    </style>
</head>
<style>
    /* Button styling */
    .info-button {
        font-size: 2rem;
        background-color: #508dce;
        color: rgb(250, 245, 245);
        border: none;
        padding: 10px 20px;
        cursor: pointer;
        border-radius: 5px;
        display: flex;
        align-items: center;
    }

    .info-button i {
        margin-right: 10px;
    }

    /* Hidden information styling */
    .hidden-info {
        display: none;
        margin-top: 20px;
        background-color: #97b1cc;
        padding: 20px;
        border: 1px solid #ddd;
        border-radius: 5px;
    }

    /* Back button styling */
    .back-button {
        font-size: 1.5rem;
        background-color: #d9534f;
        color: white;
        border: none;
        padding: 8px 16px;
        margin-top: 15px;
        cursor: pointer;
        border-radius: 5px;
    }

    /* Hover effects */
    .info-button:hover {
        background-color: #0056b3;
    }

    .back-button:hover {
        background-color: #c9302c;
    }
</style>
</head>
<body>
<!-- Info Button with Three Bullet Points -->
<button class="info-button" onclick="toggleInfo()">
    <i class="fas fa-bars"></i> Info
</button>

<!-- Hidden Info Section -->
<div class="hidden-info" id="infoSection">
    <h3></h3>
    <p><b>If you have any ideas or projects related to web development,<br>
         feel free to reach out to me via email or through the contact section</b></p>
    
    <!-- Back Button -->
    <button class="back-button" onclick="goBack()">Back</button>
</div>


<script>
   
    function toggleInfo() {
        const infoSection = document.getElementById('infoSection');
        if (infoSection.style.display === 'none' || infoSection.style.display === '') {
            infoSection.style.display = 'block';
        } else {
            infoSection.style.display = 'none';
        }
    }

    
    function goBack() {
        if (document.referrer !== "") {
          
            window.history.back();
        } else {
           
            const infoSection = document.getElementById('infoSection');
            infoSection.style.display = 'none';
        }
    }
</script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume</title>
    <style>
        body {
            background-image: url(bubble.jpg);
            background-size: cover;  
            background-position: center;  
            height: 100vh;  
            margin: 0;  
        }
    </style>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            text-align: center;
            margin-bottom: 20px;
            
        }
        h1 {
            margin: 0;
        }
        .profile-img {
            width: 180px;
            height: 250px;
            border-radius: 500%;
            margin: 10px auto;
            display: block;
           
        }
        .section {
            margin-bottom: 20px;
        }
        .section h2 {
            border-bottom: 2px solid #0e0d0d;
            padding-bottom: 5px;
            margin-bottom: 10px;
            background-color: cadetblue;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            margin-bottom: 10px;
        }
        nav {
            text-align: center;
            margin-bottom: 20px;
            background-color:rgb(214, 207, 207);
        }
        nav a {
            margin: 0 10px;
            text-decoration: none;
            color: #007BFF;
        }
        nav a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        
        <img src="Akki.Jpg" alt="Profile Picture" class="profile-img">
        <h1>Vempati Akhila</h1><br>
    </header>
</body>
<body>
    <div class="container">
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Navigation with Icons</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
        <style>
            nav {
                text-align: center;
                margin-top: 20px;
            }
            nav a {
                text-decoration: none;
                color: rgb(75, 73, 74);
                font-size: 3rem;
                margin: 0 20px;
            }
            nav a:hover {
                color: #2c94da;
            }
        </style>
    </head>
    <body>
        <nav>
            <a href="#SUMMARY"><i class="fas fa-info-circle"></i></a>
            <a href="#education"><i class="fas fa-graduation-cap"></i></a><br><br>
            <a href="#skills"><i class="fas fa-cogs"></i></a>
            <a href="#PROJECTS"><i class="fas fa-tasks"></i></a>
            <a href="#CERTIFICATES"><i class="fas fa-certificate"></i></a>
            <a href="#CONTACT"><i class="fas fa-phone"></i></a>
        </nav>
        
        <div id="SUMMARY" class="section"><br>
            <br><br><BR><BR>
            <h2>SUMMARY<BR></h2><BR>
            <p><b>A Data Science student at <B>ANURAG UNIVERSITY</B> with a passion for</p>
            <P>PYTHON, JAVA and C programming.Skilled in working within teams and <BR><BR>eager to address complex challenges through collaborative <BR><BR>problem-solving.<BR><BR>

                Enthusiastic and dedicated web developer with a strong passion for<BR><BR>designing and building responsive websites using HTML and CSS.<b>
            </p><BR><BR><BR><BR><BR><BR><BR>
        </div>
        <div id="education" class="section"><BR><BR><br><br>
            <h2>Education</h2>
            <ul>
                <li>
                    <strong> 
                         B.TECH:</strong><BR>
                        DATA SCIENCE, CGPA:9.29 <BR>
                              ANURAG UNIVERSITY <BR>
                        2020-2026<BR> 
                   <strong>INTERMEDIATE:</strong><BR> 
                       MARKS-960 <BR>
                             PRAGATHI JUNIOR CLG. <BR>
                             NALGONDA. <BR>
                  <strong>SCHOOL:</strong> <br>
                       ALPHA HIGHT SCHOOL.<br> 
                             2015-2020. <br>
                             CGPA:10<br><br><br><br><br><br>
                </li>
            </ul>
        </div>
        <div id="skills" class="section"><br><br><br><br><br><br><br>
            <br><br><br>
            <h2>Skills</h2>
            <ul>
                <li><B>Programming: </B><BR>
                    Python,Java,C, HTML and CSS</li>
                
                <li><B>Tools:</B><BR>
                    powerBI,Tableau</li>
            </ul>
        </div>
        <div id="projects" class="section"><br><br><br><br><br><br><br>
            <br><br><br>
            <h2>Projects</h2>
           <p><b>1.YOUTUBE VEDIO DOWNLOADER USING PYTHON</b></p>
        </div>
       <br><br><br><br><br><br><br><br><BR><br><br><br>

        <div id="CERTIFICATES" class="section"><br>
            <H2>CERTIFICATES</H2>
            <H3>
                <ol type="circle">
                    Qlik <br>
                    MongoDB<br>
                    HTML <br>
                    Cisco Network Basics<br>
                    Cisco Data Analytics Essentials
                </ol>
            </H3>
            <ul>
                <li>
                    <a href ="resume1.html"><p style="font-size: 24px;">CERTIFICATES </p></a>
                    
                    <br><br><br><br><br><br><br><br><br>
                </li>
            </ul>
        </div>
        <div id="CONTACT" class="section">        
                    <style>
                        /* Style for the icons */
                        .social-icons {
                            display: flex;
                            justify-content: center;
                            align-items: center;
                            gap: 20px;
                            margin-top: 50px;
                        }
                
                        .social-icons a {
                            width: 50px;
                            height: 50px;
                            transition: transform 0.3s ease;
                        }
                
                        .social-icons a:hover {
                            transform: scale(1.1); /* Slight zoom effect */
                        }
                
                        .social-icons svg {
                            width: 50px;
                            height: 50px;
                        }
                    </style>
                </head>
                <body>
                    <h2 style="text-align: center;">CONTACT</h2>
                    
                
                    <div class="social-icons">
                        <!-- Email -->
                 <a href="mailto:myemail@example.com" target="_blank">
                 <svg viewBox="0 0 24 24" fill="#D44638">
                 <path d="M12 12.713L1.198 4.501A2 2 0 012 4h20a2 2 0 01.802.501L12 12.713z"/>
                 <h6>Email</h6>
                       </svg>
                 </a>
                
                </a>
                        <!-- WhatsApp -->
                        <a href="https://wa.me/919494570994" target="_blank">
                            <svg viewBox="0 0 24 24" fill="#25D366">
                                <path d="M20.52 3.48A11.73 11.73 0 008.86 2a11.56 11.56 0 00-7.84 19.92L0 24l2.2-.58a11.64 11.64 0 005.36 1.37 11.56 11.56 0 008.92-4.4 11.6 11.6 0 003.22-8.54 11.58 11.58 0 00-2.18-7.36zm-8.27 16a9.35 9.35 0 01-4.74-1.29l-3.54.93.94-3.44a9.43 9.43 0 01-1.42-4.92 9.35 9.35 0 019.37-9.37 9.35 9.35 0 019.37 9.37 9.34 9.34 0 01-9.37 9.37z"/>
                            
                            </svg>
                            <h6>WhatsApp</h6>
                        </a>
                
                        <!-- Instagram -->
                        <a href="https://www.instagram.com/akhila_vempati/" target="_blank">
                            <svg viewBox="0 0 24 24" fill="#E4405F">
                                <path d="M12 2.2c3.2 0 3.6 0 4.8.1 1.2.1 1.9.3 2.6.6a5.6 5.6 0 012.1 1.4c.6.6 1.1 1.3 1.4 2.1.3.7.5 1.4.6 2.6.1 1.2.1 1.6.1 4.8s0 3.6-.1 4.8c-.1 1.2-.3 1.9-.6 2.6a5.6 5.6 0 01-1.4 2.1 5.6 5.6 0 01-2.1 1.4c-.7.3-1.4.5-2.6.6-1.2.1-1.6.1-4.8.1s-3.6 0-4.8-.1c-1.2-.1-1.9-.3-2.6-.6a5.6 5.6 0 01-2.1-1.4 5.6 5.6 0 01-1.4-2.1c-.3-.7-.5-1.4-.6-2.6-.1-1.2-.1-1.6-.1-4.8s0-3.6.1-4.8c.1-1.2.3-1.9.6-2.6a5.6 5.6 0 011.4-2.1 5.6 5.6 0 012.1-1.4c.7-.3 1.4-.5 2.6-.6C8.4 2.2 8.8 2.2 12 2.2z"/>
                                <h6>Instagram</h6>
                            </svg>
                        </a>
                
                        <!-- LinkedIn -->
                        <a href="https://www.linkedin.com/in/akhila-vempati-747439277" target="_blank">
                            <svg viewBox="0 0 24 24" fill="#0077b5">
                                <path d="M22.23 0H1.77C.79 0 0 .77 0 1.72v20.56c0 .95.79 1.72 1.77 1.72h20.46c.98 0 1.77-.77 1.77-1.72V1.72C24 .77 23.21 0 22.23 0zM7.14 20.54H3.56V8.8h3.58v11.74zM5.35 7.3c-1.15 0-2.08-.93-2.08-2.08 0-1.15.93-2.08 2.08-2.08s2.08.93 2.08 2.08c0 1.14-.93 2.08-2.08 2.08zm15.19 13.24h-3.57V14.4c0-1.46-.03-3.34-2.04-3.34s-2.35 1.6-2.35 3.25v6.23H8.99V8.8h3.43v1.6h.05c.48-.91 1.66-1.86 3.42-1.86 3.67 0 4.34 2.42 4.34 5.57v6.43z"/>
                                <h6>LinkedIn</h6>
                            </svg>
                        </a>
                        <!-- GitHub -->
                        <a href="https://github.com/VempatiAkhila6" target="_blank">
                            <svg viewBox="0 0 24 24" fill="#181717">
                                <path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.207 11.385.6.113.793-.262.793-.577v-2.26c-3.338.725-4.033-1.415-4.033-1.415-.546-1.387-1.333-1.757-1.333-1.757-1.087-.744.083-.729.083-.729 1.205.086 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.304 3.495.998.108-.775.418-1.304.762-1.604-2.665-.3-5.467-1.335-5.467-5.93 0-1.31.468-2.38 1.236-3.22-.123-.303-.54-1.524.117-3.176 0 0 1.008-.322 3.3 1.23a11.5 11.5 0 016.003 0c2.292-1.552 3.3-1.23 3.3-1.23.657 1.652.24 2.873.117 3.176.768.84 1.236 1.91 1.236 3.22 0 4.61-2.807 5.625-5.478 5.92.43.372.823 1.102.823 2.222v3.293c0 .32.192.694.8.576 4.768-1.586 8.207-6.082 8.207-11.385 0-6.627-5.373-12-12-12z"/>
                                <h6>GitHub</h6>
                            </svg>
                        </a></div>
                </p>
                </p>
            <BR><BR><BR><BR><BR><BR><BR>
        </div>
        
    </body>
</html>
