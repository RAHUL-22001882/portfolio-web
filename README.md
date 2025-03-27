# portfolio-web
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rahul's Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }
        body {
            background: linear-gradient(135deg, #0f0f0f, #1a1a2e);
            color: white;
            text-align: center;
            transition: background 0.3s ease-in-out;
        }
        header {
            background: rgba(30, 30, 30, 0.95);
            padding: 15px;
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 25px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s, transform 0.3s;
        }
        nav ul li a:hover {
            color: #00bcd4;
            transform: scale(1.1);
        }
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 50px;
            animation: fadeIn 1.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .hero img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 4px solid white;
            box-shadow: 0 0 30px rgba(255, 255, 255, 0.3);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .hero img:hover {
            transform: scale(1.15);
            box-shadow: 0 0 50px rgba(255, 255, 255, 0.6);
        }
        .container {
            padding: 100px 20px;
        }
        .section {
            max-width: 800px;
            margin: 30px auto;
            padding: 50px;
            background: rgba(41, 41, 41, 0.95);
            border-radius: 15px;
            box-shadow: 0 6px 25px rgba(255, 255, 255, 0.3);
            transition: transform 0.3s, box-shadow 0.3s;
            backdrop-filter: blur(20px);
        }
        .section:hover {
            transform: translateY(-12px);
            box-shadow: 0 10px 40px rgba(255, 255, 255, 0.5);
        }
        .section h2 {
            font-size: 2rem;
            margin-bottom: 15px;
            color: #00bcd4;
            text-transform: uppercase;
        }
        .toggle-btn {
            background: #00bcd4;
            color: black;
            padding: 15px 35px;
            border: none;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 10px;
            font-weight: bold;
            font-size: 18px;
            transition: background 0.3s, transform 0.3s;
        }
        .toggle-btn:hover {
            background: #008ba3;
            transform: scale(1.15);
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="home" class="hero">
        <img src="profile.jpg" alt="Rahul Profile Picture">
        <h1>Hi, I'm Rahul</h1>
        <p>AI & Web Developer | Passionate about Deep Learning & Real-Time Applications</p>
    </section>
    
    <div class="container">
        <section id="about" class="section">
            <h2>About Me</h2>
            <p>I'm a Computer Science student specializing in AI, deep learning, and web development. I love building real-world applications.</p>
        </section>
        
        <section id="projects" class="section">
            <h2>Projects</h2>
            <ul>
                <li><strong>Landslide Prediction System</strong> - AI-based real-time monitoring using satellite imagery.</li>
                <li><strong>Diabetic Retinopathy Detection</strong> - CNN model for medical image classification.</li>
            </ul>
        </section>
        
        <section id="contact" class="section">
            <h2>Contact Me</h2>
            <p>Phone: 6789022345</p>
            <p>Email: balajirahul04@gmail.com</p>
        </section>
    </div>
</body>
</html>
