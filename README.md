/* Base Styles */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    background: #ffffff; /* Fallback color */
    color: #ffffff;
    line-height: 1.6;
}

.video-background {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    min-height: 100%;
    z-index: -1;
    overflow: hidden; /* Ensure video doesn't overflow */
}

.overlay {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    min-height: 100%;
    z-index: -1;
    background: rgba(0, 0, 0, 0.5); /* Adjust transparency as needed */
}

.content {
    position: relative;
    z-index: 1;
    overflow: auto; /* Enable scrolling */
    padding: 20px;
    max-width: 1200px;
    margin: 0 auto;
}

/* Header Styles */
header {
    background: rgba(0, 0, 0, 0.188);
    color: #333;
    padding: 20px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    border-bottom: #000000 3px solid;
}

header h1 {
    margin: 0;
    font-size: 2em;
    animation: fadeInDown 10s;
}

header p {
    font-size: 1.2em;
    margin: 10px 0;
    animation: fadeInUp 10s;
}

header .profile-pic {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    border: 3px solid #000000;
    margin-bottom: 20px;
    animation: bounceIn 15s;
}

@keyframes fadeInDown {
    0% { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInUp {
    0% { opacity: 0; transform: translateY(20px); }
    100% { opacity: 1; transform: translateY(0); }
}

@keyframes bounceIn {
    0%, 20%, 40%, 60%, 80%, 100% {
        transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
    }
    0% {
        opacity: 0;
        transform: scale3d(.3, .3, .3);
    }
    20% {
        transform: scale3d(1.1, 1.1, 1.1);
    }
    40% {
        transform: scale3d(.9, .9, .9);
    }
    60% {
        opacity: 1;
        transform: scale3d(1.03, 1.03, 1.03);
    }
    80% {
        transform: scale3d(.97, .97, .97);
    }
    100% {
        opacity: 1;
        transform: scale3d(1, 1, 1);
    }
}

/* Navigation Styles */
nav {
    background: rgb(0, 0, 0);
    color: #333;
    padding: 10px 0;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

nav ul {
    padding: 0;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

nav ul li {
    margin: 0 10px;
}

nav ul li a {
    color: #24f3de;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #ffffff;
}

/* Section Styles */
section {
    padding: 50px 0;
    border: 10px solid #ffffff33;
    border-bottom: 10px solid rgba(255, 255, 255, 0.267);
    background: rgba(0, 49, 41, 0.619);
    margin-top: 20px;
    border-radius: 20px;
    max-width: 100%;
    box-sizing: border-box;
}

section h2 {
    text-align: center;
    margin: 0 0 20px;
    font-size: 2em;
    color: #44fdc6bb;
    animation: fadeIn 20s;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

.project {
    background: #24f3de55;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 20px;
    box-shadow: 0 0 40px rgba(0, 0, 0, 0.386);
    transition: transform 0.5s;
    box-sizing: border-box;
}

.project:hover {
    transform: translateY(-10px);
}

.project h3 {
    margin-top: 0;
}

.project p {
    margin-bottom: 10px;
}

.project a {
    color: #0c6a62b1;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

.project a:hover {
    color: #f3fffa5c;
}

/* Skills Styles */
#skills ul {
    padding: 0;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0;
}

#skills ul li {
    background: #24f3de;
    color: #000000;
    padding: 10px 20px;
    margin: 10px;
    border-radius: 20px;
    font-weight: bold;
    transition: transform 0.1s;
    box-sizing: border-box;
}

#skills ul li:hover {
    transform: scale(1.1);
}

/* Contact Styles */
#contact p {
    text-align: center;
}

#contact a {
    color: #ffffff81;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

#contact a:hover {
    color: #61c5ff;
}

/* Footer Styles */
footer {
    background: rgb(1, 4, 2);
    color: #24f3de;
    text-align: center;
    padding: 20px 0;
    margin-top: 20px;
}

#footertext {
    color: #24f3de; 
}

/* Responsive Styles */
@media (max-width: 1024px) {
    .content {
        padding: 10px;
    }

    header {
        padding: 15px;
    }

    header h1 {
        font-size: 1.8em;
    }
    
    header p {
        font-size: 1.1em;
    }
    
    nav ul li {
        margin: 0 5px;
    }

    section {
        padding: 30px 10px;
    }

    section h2 {
        font-size: 1.8em;
    }
    
    .project {
        padding: 15px;
    }
    
    #skills ul li {
        padding: 8px 15px;
        margin: 8px;
    }
}

@media (max-width: 768px) {
    header {
        padding: 10px;
    }

    header h1 {
        font-size: 1.5em;
    }
    
    header p {
        font-size: 1em;
    }
    
    nav ul {
        flex-direction: column;
    }

    nav ul li {
        margin: 5px 0;
    }

    section {
        padding: 20px 10px;
    }

    section h2 {
        font-size: 1.5em;
    }
    
    .project {
        padding: 10px;
    }
    
    #skills ul li {
        padding: 5px 10px;
        margin: 5px;
    }
}

@media (max-width: 480px) {
    header h1 {
        font-size: 1.2em;
    }
    
    header p {
        font-size: 0.9em;
    }

    section {
        padding: 15px 5px;
    }

    section h2 {
        font-size: 1.2em;
    }
    
    .project {
        padding: 8px;
    }
    
    #skills ul li {
        padding: 3px 8px;
        margin: 3px;
    }
}


