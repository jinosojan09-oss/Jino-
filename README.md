
<html lang="en">

<head>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Jino Sojan | Web Technology Portfolio</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background: #0b0f19;
            color: white;
            line-height: 1.6;
        }

        /* ================= NAVIGATION ================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;

            display: flex;
            justify-content: space-between;
            align-items: center;

            padding: 18px 8%;

            background: rgba(11, 15, 25, 0.90);
            backdrop-filter: blur(10px);

            border-bottom: 1px solid #252b3a;
        }

        nav .logo {
            font-size: 22px;
            font-weight: bold;
            color: #00e5ff;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        nav ul li a {
            text-decoration: none;
            color: #ddd;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #00e5ff;
        }


        /* ================= HERO ================= */

        .hero {
            min-height: 85vh;

            display: flex;
            justify-content: center;
            align-items: center;

            text-align: center;

            padding: 40px 20px;

            background:
                radial-gradient(
                    circle at top left,
                    #123b55,
                    transparent 40%
                ),

                radial-gradient(
                    circle at bottom right,
                    #30145f,
                    transparent 40%
                );
        }

        .hero-content {
            max-width: 850px;
        }

        .hero small {
            color: #00e5ff;

            font-size: 18px;

            letter-spacing: 3px;
        }

        .hero h1 {
            font-size: clamp(45px, 8vw, 85px);

            margin: 15px 0;

            background:
                linear-gradient(
                    90deg,
                    #00e5ff,
                    #8a5cff
                );

            -webkit-background-clip: text;

            color: transparent;
        }

        .hero h2 {
            font-size: 25px;

            color: #ddd;

            font-weight: normal;
        }

        .hero p {
            margin: 25px auto;

            max-width: 650px;

            color: #aaa;

            font-size: 17px;
        }

        .button {
            display: inline-block;

            margin-top: 15px;

            padding: 13px 28px;

            border-radius: 30px;

            text-decoration: none;

            color: white;

            background:
                linear-gradient(
                    90deg,
                    #00bcd4,
                    #7c4dff
                );

            transition: 0.3s;
        }

        .button:hover {

            transform: translateY(-4px);

            box-shadow:
                0 10px 30px
                rgba(0, 229, 255, 0.25);
        }


        /* ================= GENERAL SECTIONS ================= */

        section {
            padding: 80px 8%;
        }

        .section-title {

            text-align: center;

            font-size: 38px;

            margin-bottom: 15px;
        }

        .section-subtitle {

            text-align: center;

            color: #888;

            margin-bottom: 50px;
        }

        .divider {

            width: 80px;

            height: 4px;

            background:
                linear-gradient(
                    90deg,
                    #00e5ff,
                    #7c4dff
                );

            margin:
                0 auto 20px;

            border-radius: 10px;
        }


        /* ================= ABOUT ================= */

        .about-box {

            max-width: 900px;

            margin: auto;

            padding: 35px;

            background: #121827;

            border: 1px solid #252d40;

            border-radius: 20px;

            box-shadow:
                0 15px 40px
                rgba(0,0,0,0.3);
        }

        .about-box p {

            color: #bbb;

            font-size: 17px;
        }

        .highlight {

            color: #00e5ff;

            font-weight: bold;
        }


        /* ================= CARDS ================= */

        .cards {

            display: grid;

            grid-template-columns:
                repeat(
                    auto-fit,
                    minmax(230px, 1fr)
                );

            gap: 25px;

            max-width: 1100px;

            margin: auto;
        }

        .card {

            position: relative;

            padding: 30px;

            background:
                linear-gradient(
                    145deg,
                    #151c2c,
                    #0f1420
                );

            border: 1px solid #293247;

            border-radius: 20px;

            text-align: center;

            transition: 0.4s;

            overflow: hidden;
        }

        .card::before {

            content: "";

            position: absolute;

            width: 100px;

            height: 100px;

            background: #00e5ff;

            filter: blur(70px);

            opacity: 0;

            transition: 0.4s;
        }

        .card:hover::before {

            opacity: 0.2;
        }

        .card:hover {

            transform: translateY(-10px);

            border-color: #00e5ff;

            box-shadow:
                0 15px 40px
                rgba(0,229,255,0.12);
        }

        .icon {

            font-size: 45px;

            margin-bottom: 15px;
        }

        .card h3 {

            font-size: 23px;

            margin-bottom: 10px;
        }

        .card p {

            color: #999;

            margin-bottom: 20px;
        }

        .card a {

            display: inline-block;

            padding: 10px 20px;

            border:
                1px solid #00e5ff;

            border-radius: 25px;

            color: #00e5ff;

            text-decoration: none;

            transition: 0.3s;
        }

        .card a:hover {

            background: #00e5ff;

            color: #071018;
        }


        /* ================= FOOTER ================= */

        footer {

            text-align: center;

            padding: 30px;

            background: #080b12;

            color: #777;

            border-top:
                1px solid #222938;
        }

        footer span {

            color: #00e5ff;
        }


        /* ================= MOBILE ================= */

        @media (max-width: 600px) {

            nav {

                padding:
                    15px 5%;
            }

            nav ul {

                gap: 12px;
            }

            nav ul li a {

                font-size: 13px;
            }

            .hero h1 {

                font-size: 50px;
            }

            section {

                padding:
                    60px 5%;
            }

        }

    </style>

</head>


<body>


<!-- =====================================================
     NAVIGATION
===================================================== -->

<nav>

    <div class="logo">
        JS.
    </div>

    <ul>

        <li>
            <a href="#about">
                About
            </a>
        </li>

        <li>
            <a href="#certifications">
                Certifications
            </a>
        </li>

        <li>
            <a href="#projects">
                Projects
            </a>
        </li>

    </ul>

</nav>



<!-- =====================================================
     HERO SECTION
===================================================== -->

<div class="hero">

    <div class="hero-content">

        <small>
            WEB TECHNOLOGY PORTFOLIO
        </small>

        <h1>
            Jino Sojan
        </h1>

        <h2>
            3rd Year Student • RNU
        </h2>

        <p>

            Exploring the world of programming,
            web development and technology while
            building projects and developing new skills.

        </p>

        <a
            href="#certifications"
            class="button"
        >
            Explore My Work ↓
        </a>

    </div>

</div>



<!-- =====================================================
     ABOUT ME
===================================================== -->

<section id="about">

    <div class="divider"></div>

    <h2 class="section-title">
        About Me
    </h2>

    <p class="section-subtitle">
        A little introduction
    </p>


    <div class="about-box">

        <p>

            Hello! I'm
            <span class="highlight">
                Jino Sojan
            </span>,

            a third-year student at
            <span class="highlight">
                Riga Nordic University (RNU)
            </span>.

        </p>


        <br>


        <p>

            I am currently studying
            <span class="highlight">
                Web Technology
            </span>

            and developing my skills in programming,
            web design and modern technologies.

            This portfolio showcases my certifications
            and projects completed throughout my
            academic journey.

        </p>

    </div>

</section>



<!-- =====================================================
     CERTIFICATIONS
===================================================== -->

<section id="certifications">

    <div class="divider"></div>

    <h2 class="section-title">
        Certifications
    </h2>

    <p class="section-subtitle">
        Skills I've developed along the way
    </p>


    <div class="cards">


        <!-- ================= C ================= -->

        <div class="card">

            <div class="icon">
                💻
            </div>

            <h3>
                C Programming
            </h3>

            <p>

                Programming fundamentals,
                logic and problem solving.

            </p>


            <!-- YOUR C CERTIFICATE -->

            <a
                href="https://docs.google.com/presentation/d/1g2sFOqacFKGB6O42DpbULYEuvaGJuF95/edit?usp=sharing&ouid=110315652068634845696&rtpof=true&sd=true"
                target="_blank"
            >

                View Certificate →

            </a>

        </div>



        <!-- ================= PYTHON ================= -->

        <div class="card">

            <div class="icon">
                🐍
            </div>

            <h3>
                Python
            </h3>

            <p>

                Python programming,
                scripting and application development.

            </p>


            <!-- ADD PYTHON LINK HERE -->

            <a
                href="YOUR_PYTHON_DRIVE_LINK"
                target="_blank"
            >

                View Certificate →

            </a>

        </div>



        <!-- ================= CSS ================= -->

        <div class="card">

            <div class="icon">
                🎨
            </div>

            <h3>
                CSS
            </h3>

            <p>

                Web styling, layouts,
                responsive design and UI.

            </p>


            <!-- ADD CSS LINK HERE -->

            <a
                href="YOUR_CSS_DRIVE_LINK"
                target="_blank"
            >

                View Certificate →

            </a>

        </div>


    </div>

</section>



<!-- =====================================================
     PAST PROJECTS
===================================================== -->

<section id="projects">

    <div class="divider"></div>

    <h2 class="section-title">
        Past Projects
    </h2>

    <p class="section-subtitle">
        Projects from my academic journey
    </p>


    <div class="cards">


        <!-- ================= 1ST SEMESTER ================= -->

        <div class="card">

            <div class="icon">
                🚀
            </div>

            <h3>
                1st Semester
            </h3>

            <p>

                Projects, assignments and
                practical work from my first semester.

            </p>


            <!-- ADD 1ST SEMESTER LINK HERE -->

            <a
                href="YOUR_1ST_SEMESTER_LINK"
                target="_blank"
            >

                View Projects →

            </a>

        </div>



        <!-- ================= 2ND SEMESTER ================= -->

        <div class="card">

            <div class="icon">
                ⚡
            </div>

            <h3>
                2nd Semester
            </h3>

            <p>

                Academic projects and practical
                work completed during semester two.

            </p>


            <!-- ADD 2ND SEMESTER LINK HERE -->

            <a
                href="YOUR_2ND_SEMESTER_LINK"
                target="_blank"
            >

                View Projects →

            </a>

        </div>



        <!-- ================= 3RD SEMESTER ================= -->

        <div class="card">

            <div class="icon">
                🌐
            </div>

            <h3>
                3rd Semester
            </h3>

            <p>

                Web technology and other projects
                completed during semester three.

            </p>


            <!-- ADD 3RD SEMESTER LINK HERE -->

            <a
                href="YOUR_3RD_SEMESTER_LINK"
                target="_blank"
            >

                View Projects →

            </a>

        </div>


    </div>

</section>



<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

    <p>

        © 2026
        <span>
            Jino Sojan
        </span>

        | Web Technology Portfolio

    </p>

</footer>


</body>

</html>
```

