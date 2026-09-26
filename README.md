<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mark & Alchie's Funeral Services | Ormoc City, Leyte</title>

    <meta name="description"
        content="Mark & Alchie's Funeral Services provides compassionate and professional funeral assistance in Ormoc City, Leyte.">

    <style>
        /* ================================
           GENERAL SETTINGS
        ================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f8f8f8;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        button,
        input,
        textarea,
        select {
            font-family: inherit;
        }

        .container {
            width: 90%;
            max-width: 1150px;
            margin: auto;
        }

        /* ================================
           HEADER / NAVIGATION
        ================================= */

        header {
            background: #111827;
            color: white;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 3px 15px rgba(0,0,0,0.15);
        }

        .navbar {
            min-height: 75px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 21px;
            font-weight: bold;
            letter-spacing: 0.5px;
        }

        .logo span {
            color: #c9a227;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 28px;
        }

        .nav-links a {
            color: white;
            font-size: 14px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #d6b64c;
        }

        .menu-btn {
            display: none;
            font-size: 28px;
            cursor: pointer;
        }

        /* ================================
           HERO SECTION
        ================================= */

        .hero {
            min-height: 100vh;
            background:
                linear-gradient(
                    rgba(17, 24, 39, 0.94),
                    rgba(17, 24, 39, 0.94)
                );
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            padding: 120px 20px 80px;
        }

        .hero-content {
            max-width: 850px;
            margin: auto;
        }

        .hero-icon {
            width: 75px;
            height: 75px;
            border: 2px solid #c9a227;
            border-radius: 50%;
            margin: 0 auto 25px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            color: #d6b64c;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 15px;
            line-height: 1.2;
        }

        .hero h1 span {
            color: #d6b64c;
        }

        .hero p {
            font-size: 18px;
            color: #d1d5db;
            max-width: 700px;
            margin: auto;
        }

        .hero-buttons {
            margin-top: 35px;
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background: #c9a227;
            color: #111827;
        }

        .btn-primary:hover {
            background: #e0c35b;
            transform: translateY(-2px);
        }

        .btn-outline {
            border: 1px solid #d6b64c;
            color: #d6b64c;
            background: transparent;
        }

        .btn-outline:hover {
            background: #d6b64c;
            color: #111827;
        }

        /* ================================
           SECTION SETTINGS
        ================================= */

        section {
            padding: 85px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 34px;
            color: #111827;
            margin-bottom: 12px;
        }

        .section-title p {
            max-width: 650px;
            margin: auto;
            color: #666;
        }

        .gold-line {
            width: 55px;
            height: 3px;
            background: #c9a227;
            margin: 15px auto;
        }

        /* ================================
           ABOUT
        ================================= */

        .about {
            background: white;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 55px;
            align-items: center;
        }

        .about-text h3 {
            font-size: 28px;
            color: #111827;
            margin-bottom: 18px;
        }

        .about-text p {
            color: #555;
            margin-bottom: 15px;
        }

        .about-boxes {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        .about-box {
            background: #f4f4f4;
            padding: 25px;
            border-left: 4px solid #c9a227;
            border-radius: 5px;
        }

        .about-box h4 {
            color: #111827;
            margin-bottom: 7px;
        }

        .about-box p {
            font-size: 14px;
            color: #666;
        }

        /* ================================
           SERVICES
        ================================= */

        .services {
            background: #f4f5f7;
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
        }

        .service-card {
            background: white;
            padding: 30px;
            border-radius: 7px;
            text-align: center;
            border: 1px solid #e5e5e5;
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-7px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
        }

        .service-icon {
            width: 58px;
            height: 58px;
            border-radius: 50%;
            background: #111827;
            color: #d6b64c;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 18px;
            font-size: 23px;
        }

        .service-card h3 {
            color: #111827;
            margin-bottom: 12px;
        }

        .service-card p {
            color: #666;
            font-size: 14px;
        }

        /* ================================
           PACKAGES
        ================================= */

        .packages {
            background: white;
        }

        .package-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .package-card {
            border: 1px solid #ddd;
            border-radius: 7px;
            overflow: hidden;
            background: white;
            transition: 0.3s;
        }

        .package-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
        }

        .package-header {
            background: #111827;
            color: white;
            text-align: center;
            padding: 25px;
        }

        .package-header h3 {
            font-size: 22px;
        }

        .package-header p {
            color: #d6b64c;
            margin-top: 8px;
            font-weight: bold;
        }

        .package-body {
            padding: 25px;
        }

        .package-body ul {
            list-style: none;
        }

        .package-body li {
            padding: 9px 0;
            border-bottom: 1px solid #eee;
            font-size: 14px;
            color: #555;
        }

        .package-body li::before {
            content: "✓";
            color: #b18c16;
            font-weight: bold;
            margin-right: 9px;
        }

        .package-note {
            text-align: center;
            margin-top: 30px;
            color: #777;
            font-size: 14px;
        }

        /* ================================
           BOOKING
        ================================= */

        .booking {
            background: #f4f5f7;
        }

        .booking-wrapper {
            max-width: 850px;
            margin: auto;
            background: white;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.07);
        }

        .form-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .form-group {
            margin-bottom: 5px;
        }

        .form-group.full {
            grid-column: 1 / -1;
        }

        label {
            display: block;
            font-weight: bold;
            font-size: 14px;
            color: #333;
            margin-bottom: 7px;
        }

        input,
        select,
        textarea {
            width: 100%;
            padding: 13px;
            border: 1px solid #d5d5d5;
            border-radius: 5px;
            outline: none;
            font-size: 14px;
        }

        input:focus,
        select:focus,
        textarea:focus {
            border-color: #c9a227;
        }

        textarea {
            resize: vertical;
            min-height: 120px;
        }

        .form-submit {
            text-align: center;
            margin-top: 25px;
        }

        .success-message {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background: #ecfdf5;
            color: #166534;
            border: 1px solid #bbf7d0;
            border-radius: 5px;
            text-align: center;
        }

        /* ================================
           CONTACT
        ================================= */

        .contact {
            background: #111827;
            color: white;
        }

        .contact .section-title h2 {
            color: white;
        }

        .contact .section-title p {
            color: #cbd5e1;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .contact-card {
            text-align: center;
            padding: 30px 20px;
            border: 1px solid #374151;
            border-radius: 7px;
        }

        .contact-card .contact-icon {
            font-size: 28px;
            color: #d6b64c;
            margin-bottom: 12px;
        }

        .contact-card h3 {
            margin-bottom: 8px;
        }

        .contact-card p {
            color: #cbd5e1;
            font-size: 14px;
        }

        /* ================================
           FOOTER
        ================================= */

        footer {
            background: #080c14;
            color: #9ca3af;
            text-align: center;
            padding: 25px 15px;
            font-size: 13px;
        }

        footer strong {
            color: #d6b64c;
        }

        /* ================================
           MOBILE
        ================================= */

        @media (max-width: 850px) {

            .menu-btn {
                display: block;
            }

            .nav-links {
                position: absolute;
                top: 75px;
                left: 0;
                width: 100%;
                background: #111827;
                flex-direction: column;
                text-align: center;
                gap: 0;
                display: none;
            }

            .nav-links.active {
                display: flex;
            }

            .nav-links li {
                border-top: 1px solid #374151;
            }

            .nav-links a {
                display: block;
                padding: 15px;
            }

            .hero h1 {
                font-size: 38px;
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .service-grid,
            .package-grid {
                grid-template-columns: 1fr 1fr;
            }

            .contact-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 600px) {

            .container {
                width: 92%;
            }

            section {
                padding: 65px 0;
            }

            .hero h1 {
                font-size: 31px;
            }

            .hero p {
                font-size: 16px;
            }

            .hero-buttons {
                flex-direction: column;
            }

            .hero-buttons .btn {
                width: 100%;
            }

            .about-boxes {
                grid-template-columns: 1fr;
            }

            .service-grid,
            .package-grid,
            .form-grid {
                grid-template-columns: 1fr;
            }

            .form-group.full {
                grid-column: auto;
            }

            .booking-wrapper {
                padding: 25px 18px;
            }

            .section-title h2 {
                font-size: 29px;
            }
        }
    </style>
</head>

<body>

    <!-- ================================
         NAVIGATION
    ================================= -->

    <header>
        <div class="container navbar">

            <div class="logo">
                Mark <span>&</span> Alchie's
            </div>

            <div class="menu-btn" id="menuBtn">
                ☰
            </div>

            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#packages">Packages</a></li>
                <li><a href="#booking">Booking</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

        </div>
    </header>


    <!-- ================================
         HOME
    ================================= -->

    <section class="hero" id="home">

        <div class="hero-content">

            <div class="hero-icon">
                ✦
            </div>

            <h1>
                Mark <span>&</span> Alchie's
                <br>
                Funeral Services
            </h1>

            <p>
                Compassionate and professional funeral assistance
                for families in Ormoc City, Leyte.
                We are here to help provide dignity, respect,
                and care during difficult times.
            </p>

            <div class="hero-buttons">
                <a href="#booking" class="btn btn-primary">
                    Request Assistance
                </a>

                <a href="#services" class="btn btn-outline">
                    View Our Services
                </a>
            </div>

        </div>

    </section>


    <!-- ================================
         ABOUT
    ================================= -->

    <section class="about" id="about">

        <div class="container">

            <div class="section-title">

                <h2>About Us</h2>

                <div class="gold-line"></div>

                <p>
                    Providing respectful and compassionate funeral
                    assistance to families in Ormoc City.
                </p>

            </div>


            <div class="about-grid">

                <div class="about-text">

                    <h3>Serving Families With Care and Respect</h3>

                    <p>
                        Mark & Alchie's Funeral Services is a
                        proposed funeral service provider serving
                        families in Ormoc City, Leyte.
                    </p>

                    <p>
                        We understand that losing a loved one is
                        one of life's most difficult experiences.
                        Our goal is to assist families with funeral
                        arrangements while treating every family
                        with dignity, compassion, and respect.
                    </p>

                    <p>
                        From preparation and coordination to funeral
                        arrangements, our services are designed to
                        make the process more organized and manageable
                        for grieving families.
                    </p>

                </div>


                <div class="about-boxes">

                    <div class="about-box">
                        <h4>Compassion</h4>
                        <p>
                            We approach every family with understanding,
                            patience, and respect.
                        </p>
                    </div>

                    <div class="about-box">
                        <h4>Dignity</h4>
                        <p>
                            We aim to provide respectful arrangements
                            for every departed loved one.
                        </p>
                    </div>

                    <div class="about-box">
                        <h4>Professionalism</h4>
                        <p>
                            We strive to provide organized and
                            dependable funeral assistance.
                        </p>
                    </div>

                    <div class="about-box">
                        <h4>Community</h4>
                        <p>
                            We aim to serve families within
                            Ormoc City and nearby areas.
                        </p>
                    </div>

                </div>

            </div>

        </div>

    </section>


    <!-- ================================
         SERVICES
    ================================= -->

    <section class="services" id="services">

        <div class="container">

            <div class="section-title">

                <h2>Our Services</h2>

                <div class="gold-line"></div>

                <p>
                    Funeral assistance and arrangements designed
                    to help families during times of loss.
                </p>

            </div>


            <div class="service-grid">

                <div class="service-card">

                    <div class="service-icon">✦</div>

                    <h3>Funeral Arrangements</h3>

                    <p>
                        Assistance with organizing funeral
                        arrangements according to the family's
                        preferences and needs.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">♥</div>

                    <h3>Embalming Assistance</h3>

                    <p>
                        Coordination and assistance for preparation
                        and preservation services through qualified
                        personnel.
                    </p>

                </div>


                <div c
