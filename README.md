<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Video background -->
    <div class="video-background">
        <video autoplay muted loop poster="your-background.jpg" id="bgvid">
            <source src="background.mp4" type="video/mp4">
        </video>
    </div>
    
    <!-- Overlay to control transparency -->
    <div class="overlay"></div>

    <!-- Background audio -->
    <audio autoplay loop>
        <source src="background.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>


    <!-- Content -->
    <div class="content">
        <header>
            <div class="container">
                <img src="picture.jpg" alt="Profile Picture" class="profile-pic">
                <h1>Mateo Arumugam</h1>
                <p>Software Developer | JavaScript Enthusiast | Front-End Specialist</p>
            </div>
        </header>
        
        <nav>
            <ul class="container">
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    
        <section id="about" class="container">
            <h2>About Me</h2>
            <p>I'm a software engineer specializing in front-end development with a focus on JavaScript. I enjoy creating sleek, user-friendly interfaces and solving complex challenges to enhance user experiences. With a passion for continuous learning and innovation, I thrive in collaborative environments, pushing boundaries to deliver high-quality solutions.</p>
        </section>
    
        <section id="projects" class="container">
            <h2>Projects</h2>
            <div class="project">
                <h3>Project One: A Memory Card Game</h3>
                <p>I developed a dynamic memory card game where players match pairs within a grid. Features include interactive gameplay with animated card flips, responsive design, and endgame feedback. Designed to challenge memory skills while demonstrating proficiency in JavaScript and front-end development. <a href="https://mateoarumugam.github.io/MemoryCardGame-by-Mateo-Arumugam/">View more</a></p>
            </div>
            <div class="project">
                <h3>Project Two: Up and Coming</h3>
                <p>Stay tuned to see what's next. <a href="#">View more</a></p>
            </div>
        </section>
    
        <section id="skills" class="container">
            <h2>Skills</h2>
            <ul>
                <li>JavaScript</li>
                <li>React</li>
                <li>CSS3</li>
                <li>HTML5</li>
                <li>Git</li>
                <li>Node.js</li>
            </ul>
        </section>
    
        <section id="contact" class="container">
            <h2>Contact</h2>
            <p>Email: <a href="mailto:mateoarumugam@gmail.com">mateoarumugam@gmail.com</a></p>
            <p>LinkedIn: <a href="https://www.linkedin.com/public-profile/settings?trk=d_flagship3_profile_self_view_public_profile">@MateoArumugam</a></p>
            <p>GitHub: <a href="https://github.com/MateoArumugam">@MateoArumugam</a></p>
        </section>
    
        <footer>
            <div class="container">
                <p id = "footertext">&copy; 2024 Mateo Arumugam. All Rights Reserved.</p>
            </div>
        </footer>
    </div>

    <!-- JavaScript for video playback -->
    <script>
    document.addEventListener('DOMContentLoaded', function() {
        var vid = document.getElementById('bgvid');
        vid.playbackRate = 1; // Adjust playback rate if needed
    });
    </script>
</body>
</html>
