# Project
Vacation home

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>T.A.T.A. | San Antonio Vacation Homes</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        /* Basic Reset */
        * { 
            margin: 0; 
            padding: 0; 
            box-sizing: border-box; 
            font-family: Arial, sans-serif; 
        }

        body { 
            line-height: 1.6; 
            background-color: #f5f5f5; 
            color: #333; 
        }

        /* Header */
        header { 
            background: #4a90e2; 
            color: white; 
            padding: 1rem; 
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1000px;
            margin: auto;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        /* Hero Section */
        .hero {
            background: 
                linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
                url('https://images.unsplash.com/photo-1505691938895-1758d7feb511') no-repeat center center/cover;
            height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 1rem;
            overflow: hidden;
        }

        /* Fade-in Animation */
        .hero h1,
        .hero p,
        .hero .btn {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 1s forwards;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation-delay: 0.3s;
        }

        .hero p {
            max-width: 700px;
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
            animation-delay: 0.6s;
        }

        .hero .btn {
            display: inline-block;
            background: #4a90e2;
            color: white;
            padding: 0.7rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s ease, background 0.3s ease;
            animation-delay: 0.9s;
        }

        /* Button Hover Effect */
        .hero .btn:hover {
            background: #357ab8;
            transform: scale(1.05);
        }

        /* Keyframes for Fade-in Up */
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Sections */
        .section {
            padding: 4rem 1rem;
            max-width: 1000px;
            margin: auto;
            text-align: center;
        }

        h2 {
            margin-bottom: 2rem;
            font-size: 2rem;
            color: #4a90e2;
        }

        /* Contact Form */
        form {
            max-width: 500px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        input, textarea {
            padding: 0.7rem;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        button {
            background: #4a90e2;
            color: white;
            border: none;
            padding: 0.7rem;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
        }

        button:hover {
            background: #357ab8;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem 1rem;
            background: #333;
            color: white;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 1rem;
            }

            .nav-links {
                flex-direction: column;
                align-items: center;
            }

            .hero h1 {
                font-size: 2.2rem;
            }

            .hero p {
                font-size: 1rem;
            }
        }
    </style>
</head>

<body>

    <!-- Navigation -->
    <header>
        <nav class="navbar">
            <div class="logo">T.A.T.A.</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Welcome to T.A.T.A.</h1>
        <p>
            Where comfort meets convenience in the heart of San Antonio, Texas.
            Our charming vacation homes, apartments, and retreats are designed
            to help you relax and explore.
        </p>
        <a href="#contact" class="btn">Book Your Stay</a>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <h2>About Us</h2>
        <p>
            Hello and welcome! My name is Tanya, and I’m excited to be your host
            during your stay in San Antonio. As a passionate traveler, I understand
            how important it is to feel at home wherever you are.
        </p>
        <p>
            T.A.T.A. was created to be a cozy, welcoming space where guests can
            relax and enjoy a seamless stay. I take pride in offering clean,
            comfortable, and fully equipped accommodations to make your visit
            memorable.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Us</h2>
        <form>
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <input type="tel" name="phone" placeholder="Your Phone Number (Optional)">
            <textarea name="message" rows="4" placeholder="Write your message here..."></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2026 T.A.T.A. All rights reserved.</p>
    </footer>

</body>
</html>
