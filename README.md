<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Page</title>
    <style>
        /* Reset default styles */
        body, h1, h2, h3, p, a, ul {
            margin: 0;
            padding: 0;
            text-decoration: none;
            color: inherit;
            list-style: none;
        }

        /* General body styles */
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #e3fdfd 0%, #cbf1f5 50%, #a6e3e9 100%);
			background: url('background.jpg') no-repeat center center/cover;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            min-height: 100vh;
            padding: 20px;
            box-sizing: border-box;
        }

        /* Container for all cards */
        .container {
            max-width: 1000px;
            width: 100%;
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }

        /* Profile header section */
        .profile-header {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #2980b9 0%, #3498db 100%);
            border-radius: 10px 10px 0 0;
            color: white;
        }

        .profile-img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            border: 5px solid white;
            margin-bottom: 15px;
        }

        .name {
            font-size: 32px;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .title {
            font-size: 20px;
            font-weight: normal;
            color: #ecf0f1;
        }

        /* Section titles */
        .section-title {
            font-size: 24px;
            font-weight: bold;
            color: #34495e;
            margin-bottom: 15px;
        }

        /* Bio section */
        .bio-section {
            padding: 20px;
            background-color: #f7f9f9;
            border-radius: 10px;
        }

        .bio {
            font-size: 16px;
            color: #555555;
            line-height: 1.6;
        }

        /* Social links section */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            font-size: 16px;
            color: white;
            padding: 10px 15px;
            background-color: #2c3e50;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .social-link:hover {
            background-color: #34495e;
        }

        /* Information cards */
        .info-card {
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .info-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }

        /* Skills list */
        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 10px;
        }

        .skill-item {
            background-color: #16a085;
            color: white;
            padding: 8px 16px;
            border-radius: 5px;
            font-size: 14px;
        }

        /* Experience items */
        .experience-item {
            margin-bottom: 20px;
        }

        .experience-title {
            font-size: 18px;
            font-weight: bold;
            color: #34495e;
        }

        .experience-company {
            font-size: 16px;
            color: #7f8c8d;
            margin-bottom: 5px;
        }

        .experience-description {
            font-size: 14px;
            color: #555555;
            line-height: 1.6;
        }

        /* Contact details */
        .contact-info {
            font-size: 16px;
            color: #34495e;
            margin-bottom: 10px;
        }

        .contact-card {
            background-color: #f2f2f2;
            border-left: 5px solid #16a085;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Profile Header -->
        <div class="profile-header">
            <!--<img src="profile.jpg" alt="Profile Picture" class="profile-img">-->
            <h1 class="name">Vijaya Kumar</h1>
            <p class="title">Cyber security professional</p>
        </div>

        <!-- Introduction Section -->
        <div class="bio-section info-card">
            <h2 class="section-title">Introduction</h2>
            <p class="bio">
                Passionate web developer with 5 years of experience in creating dynamic and responsive websites. Expert in HTML, CSS, JavaScript, and React.js.
            </p>
            <div class="social-links">
                <a href="https://twitter.com/johndoe" target="_blank" class="social-link">Twitter</a>
                <a href="https://linkedin.com/in/johndoe" target="_blank" class="social-link">LinkedIn</a>
                <a href="https://github.com/johndoe" target="_blank" class="social-link">GitHub</a>
            </div>
        </div>

        <!-- Skills Section -->
        <div class="info-card">
            <h2 class="section-title">Skills</h2>
            <ul class="skills-list">
                <li class="skill-item">HTML & CSS</li>
                <li class="skill-item">JavaScript</li>
                <li class="skill-item">React.js</li>
                <li class="skill-item">Node.js</li>
                <li class="skill-item">Git & GitHub</li>
                <li class="skill-item">Responsive Design</li>
            </ul>
        </div>

        <!-- Experience Section -->
        <div class="info-card">
            <h2 class="section-title">Experience</h2>
            <div class="experience-item">
                <h3 class="experience-title">Senior Web Developer</h3>
                <p class="experience-company">XYZ Company, 2020 - Present</p>
                <p class="experience-description">Leading the front-end team in developing scalable and high-performance web applications using React.js and modern JavaScript frameworks.</p>
            </div>
            <div class="experience-item">
                <h3 class="experience-title">Web Developer</h3>
                <p class="experience-company">ABC Corp, 2017 - 2020</p>
                <p class="experience-description">Developed and maintained responsive websites, collaborating closely with designers and back-end developers to deliver seamless user experiences.</p>
            </div>
        </div>

        <!-- Contact Section -->
        <div class="info-card contact-card">
            <h2 class="section-title">Contact</h2>
            <p class="contact-info">Email: johndoe@example.com</p>
            <p class="contact-info">Phone: +123 456 7890</p>
            <p class="contact-info">Location: San Francisco, CA</p>
        </div>
    </div>
</body>
</html>

