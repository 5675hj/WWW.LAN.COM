<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Memelistic Empire | Luxury Wig Making, Styling & Training Academy Lagos</title>
    <meta name="description" content="Premier luxury wig brand and training academy in Lagos, Nigeria. Masterclass wig making, revamping, installation, and custom wigs.">
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* --- CSS VARIABLES & RESET --- */
        :root {
            --white: #ffffff;
            --cream: #FFF8F2;
            --champagne-gold: #D4AF37;
            --gold-light: #F4E8C1;
            --gold-dark: #AA820A;
            --light-beige: #F9F5F0;
            --soft-brown: #5C4033;
            --warm-nude: #E8D8CE;
            --elegant-grey: #666666;
            --text-dark: #222222;
            --glass-bg: rgba(255, 255, 255, 0.75);
            --glass-border: rgba(212, 175, 55, 0.25);
            --shadow-soft: 0 10px 30px rgba(92, 64, 51, 0.08);
            --shadow-gold: 0 10px 25px rgba(212, 175, 55, 0.2);
            --transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--cream);
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden;
        }

        h1, h2, h3, h4, .serif-font {
            font-family: 'Cormorant Garamond', serif;
            font-weight: 700;
            letter-spacing: -0.02em;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        ul {
            list-style: none;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
            object-fit: cover;
        }

        /* --- PRELOADER --- */
        #loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--cream);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 0.6s ease, visibility 0.6s ease;
        }

        .loader-ring {
            width: 80px;
            height: 80px;
            border: 3px solid var(--warm-nude);
            border-top: 3px solid var(--champagne-gold);
            border-radius: 50%;
            animation: spin 1s linear infinite;
        }

        .loader-text {
            margin-top: 20px;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.5rem;
            color: var(--soft-brown);
            letter-spacing: 2px;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* --- BUTTONS & GLASS CARDS --- */
        .btn-gold {
            background: linear-gradient(135deg, var(--champagne-gold), var(--gold-dark));
            color: var(--white);
            padding: 14px 32px;
            border-radius: 50px;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            box-shadow: var(--shadow-gold);
            transition: var(--transition);
            border: none;
            cursor: pointer;
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 1px;
        }

        .btn-gold:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(212, 175, 55, 0.4);
            color: var(--white);
        }

        .btn-outline {
            background: transparent;
            color: var(--soft-brown);
            border: 2px solid var(--champagne-gold);
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            transition: var(--transition);
            cursor: pointer;
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 1px;
        }

        .btn-outline:hover {
            background: var(--champagne-gold);
            color: var(--white);
            transform: translateY(-3px);
        }

        .glass-card {
            background: var(--glass-bg);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid var(--glass-border);
            border-radius: 20px;
            box-shadow: var(--shadow-soft);
        }

        /* --- HEADER & NAVIGATION --- */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            transition: var(--transition);
            padding: 20px 0;
        }

        header.scrolled {
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(10px);
            padding: 12px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
        }

        .nav-container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2rem;
            font-weight: 700;
            color: var(--soft-brown);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo span {
            color: var(--champagne-gold);
        }

        .nav-links {
            display: flex;
            align-items: center;
            gap: 30px;
        }

        .nav-links a {
            font-size: 0.95rem;
            font-weight: 500;
            color: var(--text-dark);
            transition: var(--transition);
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--champagne-gold);
            transition: var(--transition);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .menu-toggle {
            display: none;
            font-size: 1.5rem;
            color: var(--soft-brown);
            cursor: pointer;
        }

        /* --- HERO SECTION --- */
        .hero {
            min-height: 100vh;
            padding: 140px 25px 80px;
            display: flex;
            align-items: center;
            position: relative;
            background: linear-gradient(135deg, rgba(255, 248, 242, 0.9), rgba(249, 245, 240, 0.8)), url('https://i.ibb.co/qLddXYBK/Screenshot-20260727-094548-Instagram-Lite.jpg');
            background-size: cover;
            background-position: center;
            overflow: hidden;
        }

        .hero-container {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            gap: 50px;
            align-items: center;
            width: 100%;
        }

        .hero-content h1 {
            font-size: 3.8rem;
            line-height: 1.1;
            color: var(--soft-brown);
            margin-bottom: 20px;
        }

        .hero-content h1 span {
            color: var(--champagne-gold);
            font-style: italic;
        }

        .hero-content p {
            font-size: 1.15rem;
            color: var(--elegant-grey);
            margin-bottom: 35px;
            max-width: 580px;
        }

        .hero-cta {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            margin-bottom: 40px;
        }

        .hero-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            max-width: 500px;
        }

        .stat-badge {
            padding: 15px 20px;
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 0.9rem;
            font-weight: 600;
            color: var(--soft-brown);
        }

        .stat-badge i {
            color: var(--champagne-gold);
            font-size: 1.2rem;
        }

        .hero-image-wrapper {
            position: relative;
        }

        .hero-img-main {
            width: 100%;
            height: 520px;
            border-radius: 30px;
            box-shadow: var(--shadow-soft);
            border: 4px solid var(--white);
        }

        .floating-card {
            position: absolute;
            bottom: -20px;
            left: -30px;
            padding: 20px 25px;
            max-width: 260px;
            animation: float 4s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-12px); }
        }

        /* --- SECTION HEADINGS --- */
        .section-header {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 60px;
        }

        .section-subtitle {
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 3px;
            color: var(--champagne-gold);
            font-weight: 700;
            margin-bottom: 10px;
            display: block;
        }

        .section-title {
            font-size: 2.8rem;
            color: var(--soft-brown);
            line-height: 1.2;
        }

        /* --- ABOUT SECTION --- */
        .about-section {
            padding: 100px 25px;
            background: var(--white);
        }

        .about-container {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .about-gallery-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .about-img {
            border-radius: 20px;
            height: 260px;
            width: 100%;
            transition: var(--transition);
        }

        .about-img:hover {
            transform: scale(1.03);
        }

        .about-content h2 {
            font-size: 2.8rem;
            color: var(--soft-brown);
            margin-bottom: 20px;
        }

        .about-content p {
            color: var(--elegant-grey);
            margin-bottom: 25px;
        }

        .services-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }

        .tag {
            background: var(--light-beige);
            border: 1px solid var(--warm-nude);
            padding: 8px 18px;
            border-radius: 30px;
            font-size: 0.85rem;
            color: var(--soft-brown);
            font-weight: 500;
        }

        /* --- SERVICES SECTION --- */
        .services-section {
            padding: 100px 25px;
            background: var(--cream);
        }

        .services-grid {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        .service-card {
            padding: 40px 30px;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .service-card:hover {
            transform: translateY(-10px);
            border-color: var(--champagne-gold);
        }

        .service-icon {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: var(--light-beige);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--champagne-gold);
            margin-bottom: 25px;
            border: 1px solid var(--warm-nude);
        }

        .service-card h3 {
            font-size: 1.8rem;
            color: var(--soft-brown);
            margin-bottom: 12px;
        }

        .service-card p {
            color: var(--elegant-grey);
            font-size: 0.95rem;
        }

        /* --- WIG GALLERY SECTION --- */
        .wig-gallery-section {
            padding: 100px 25px;
            background: var(--white);
        }

        .gallery-grid {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }

        .wig-card {
            border-radius: 20px;
            overflow: hidden;
            position: relative;
            background: var(--cream);
            border: 1px solid var(--warm-nude);
            transition: var(--transition);
        }

        .wig-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-soft);
        }

        .wig-img-box {
            position: relative;
            height: 320px;
            overflow: hidden;
        }

        .wig-img-box img {
            width: 100%;
            height: 100%;
            transition: transform 0.6s ease;
        }

        .wig-card:hover .wig-img-box img {
            transform: scale(1.08);
        }

        .wig-info {
            padding: 20px;
            text-align: center;
        }

        .wig-info h4 {
            font-size: 1.4rem;
            color: var(--soft-brown);
            margin-bottom: 15px;
        }

        .wig-actions {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        .btn-sm {
            padding: 8px 16px;
            font-size: 0.75rem;
            border-radius: 20px;
        }

        /* --- ACADEMY / TRAINING SECTION --- */
        .academy-section {
            padding: 100px 25px;
            background: linear-gradient(180deg, var(--cream) 0%, var(--light-beige) 100%);
        }

        .academy-banner {
            max-width: 1280px;
            margin: 0 auto 60px;
            padding: 50px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
            background: var(--white);
            border-radius: 30px;
            border: 2px solid var(--champagne-gold);
        }

        .academy-details h3 {
            font-size: 2.2rem;
            color: var(--soft-brown);
            margin-bottom: 20px;
        }

        .price-badge {
            display: inline-block;
            background: var(--light-beige);
            padding: 10px 20px;
            border-radius: 30px;
            margin-bottom: 20px;
        }

        .price-badge .amount {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--champagne-gold);
        }

        .academy-meta {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin-bottom: 30px;
        }

        .meta-item {
            font-size: 0.9rem;
            color: var(--text-dark);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .meta-item i {
            color: var(--champagne-gold);
        }

        .curriculum-grid {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 20px;
        }

        .curriculum-item {
            padding: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .curriculum-item i {
            font-size: 1.2rem;
            color: var(--champagne-gold);
        }

        /* --- TESTIMONIALS & GRADUATES --- */
        .testimonials-section {
            padding: 100px 25px;
            background: var(--white);
        }

        .slider-container {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
            padding: 20px 0;
        }

        .testimonial-track {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }

        .testimonial-slide {
            min-width: 100%;
            padding: 40px;
            text-align: center;
        }

        .student-avatar {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin: 0 auto 20px;
            border: 3px solid var(--champagne-gold);
        }

        .testimonial-text {
            font-size: 1.15rem;
            font-style: italic;
            color: var(--elegant-grey);
            margin-bottom: 20px;
        }

        .student-name {
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--soft-brown);
        }

        .slider-controls {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }

        .slider-btn {
            width: 45px;
            height: 45px;
            border-radius: 50%;
            border: 1px solid var(--champagne-gold);
            background: transparent;
            color: var(--soft-brown);
            cursor: pointer;
            transition: var(--transition);
        }

        .slider-btn:hover {
            background: var(--champagne-gold);
            color: var(--white);
        }

        /* --- WHY CHOOSE US --- */
        .why-us-section {
            padding: 100px 25px;
            background: var(--cream);
        }

        .why-grid {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .why-card {
            padding: 30px;
            text-align: center;
            transition: var(--transition);
        }

        .why-card:hover {
            transform: translateY(-5px);
        }

        .why-card i {
            font-size: 2.2rem;
            color: var(--champagne-gold);
            margin-bottom: 15px;
        }

        .why-card h4 {
            font-size: 1.4rem;
            color: var(--soft-brown);
            margin-bottom: 10px;
        }

        /* --- MASONRY GALLERY --- */
        .masonry-section {
            padding: 100px 25px;
            background: var(--white);
        }

        .masonry-grid {
            max-width: 1280px;
            margin: 0 auto;
            columns: 4 250px;
            column-gap: 20px;
        }

        .masonry-item {
            margin-bottom: 20px;
            break-inside: avoid;
            border-radius: 15px;
            overflow: hidden;
            position: relative;
            cursor: pointer;
        }

        .masonry-item img {
            width: 100%;
            transition: var(--transition);
        }

        .masonry-item:hover img {
            transform: scale(1.05);
        }

        .masonry-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(92, 64, 51, 0.4);
            opacity: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            font-size: 1.5rem;
            transition: var(--transition);
        }

        .masonry-item:hover .masonry-overlay {
            opacity: 1;
        }

        /* --- FORMS & MODALS --- */
        .forms-container-section {
            padding: 100px 25px;
            background: var(--light-beige);
        }

        .forms-wrapper {
            max-width: 1100px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }

        .form-box {
            padding: 40px;
            background: var(--white);
            border-radius: 25px;
            box-shadow: var(--shadow-soft);
            border: 1px solid var(--warm-nude);
        }

        .form-box h3 {
            font-size: 2rem;
            color: var(--soft-brown);
            margin-bottom: 20px;
            text-align: center;
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 6px;
            color: var(--soft-brown);
        }

        .form-control {
            width: 100%;
            padding: 12px 18px;
            border-radius: 10px;
            border: 1px solid var(--warm-nude);
            background: var(--cream);
            font-family: inherit;
            font-size: 0.95rem;
            transition: var(--transition);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--champagne-gold);
            background: var(--white);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        /* --- FAQ SECTION --- */
        .faq-section {
            padding: 100px 25px;
            background: var(--white);
        }

        .faq-accordion {
            max-width: 800px;
            margin: 0 auto;
        }

        .faq-item {
            margin-bottom: 15px;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid var(--warm-nude);
        }

        .faq-header {
            padding: 20px;
            background: var(--cream);
            font-weight: 600;
            color: var(--soft-brown);
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .faq-body {
            padding: 0 20px;
            max-height: 0;
            overflow: hidden;
            transition: all 0.3s ease;
            background: var(--white);
        }

        .faq-item.active .faq-body {
            padding: 20px;
            max-height: 200px;
        }

        .faq-item.active .faq-header i {
            transform: rotate(180deg);
        }

        /* --- CONTACT & FOOTER --- */
        .contact-section {
            padding: 100px 25px;
            background: var(--cream);
        }

        .contact-grid {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        .contact-item {
            display: flex;
            gap: 20px;
            align-items: flex-start;
        }

        .contact-item i {
            font-size: 1.5rem;
            color: var(--champagne-gold);
            background: var(--white);
            padding: 15px;
            border-radius: 50%;
            box-shadow: var(--shadow-soft);
        }

        .map-box {
            width: 100%;
            height: 100%;
            min-height: 300px;
            border-radius: 20px;
            overflow: hidden;
            border: 1px solid var(--warm-nude);
        }

        footer {
            background: var(--soft-brown);
            color: var(--white);
            padding: 70px 25px 30px;
        }

        .footer-container {
            max-width: 1280px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 2fr 1fr 1fr 1.5fr;
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2.2rem;
            color: var(--champagne-gold);
            margin-bottom: 15px;
        }

        .footer-links h5 {
            font-size: 1.2rem;
            color: var(--champagne-gold);
            margin-bottom: 20px;
        }

        .footer-links ul li {
            margin-bottom: 10px;
        }

        .footer-links ul li a {
            color: var(--warm-nude);
            transition: var(--transition);
        }

        .footer-links ul li a:hover {
            color: var(--champagne-gold);
            padding-left: 5px;
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-icons a {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255,255,255,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            transition: var(--transition);
        }

        .social-icons a:hover {
            background: var(--champagne-gold);
            color: var(--soft-brown);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: var(--warm-nude);
            font-size: 0.85rem;
        }

        /* --- FLOATING BUTTONS --- */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 60px;
            height: 60px;
            background-color: #25d366;
            color: var(--white);
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
        }

        .back-to-top {
            position: fixed;
            bottom: 100px;
            right: 35px;
            width: 45px;
            height: 45px;
            background: var(--champagne-gold);
            color: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            opacity: 0;
            visibility: hidden;
            transition: var(--transition);
            z-index: 999;
        }

        .back-to-top.show {
            opacity: 1;
            visibility: visible;
        }

        /* --- LIGHTBOX MODAL --- */
        .lightbox-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 2000;
            display: none;
            align-items: center;
            justify-content: center;
        }

        .lightbox-content {
            max-width: 90%;
            max-height: 85%;
            border-radius: 10px;
        }

        .lightbox-close {
            position: absolute;
            top: 25px;
            right: 35px;
            color: var(--white);
            font-size: 2.5rem;
            cursor: pointer;
        }

        /* --- RESPONSIVE MEDIA QUERIES --- */
        @media (max-width: 992px) {
            .hero-container, .about-container, .academy-banner, .forms-wrapper, .contact-grid, .footer-container {
                grid-template-columns: 1fr;
            }

            .hero-content h1 {
                font-size: 2.8rem;
            }

            .menu-toggle {
                display: block;
            }

            .nav-links {
                position: fixed;
                top: 75px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 75px);
                background: var(--cream);
                flex-direction: column;
                justify-content: center;
                transition: var(--transition);
            }

            .nav-links.active {
                left: 0;
            }

            .hero {
                padding-top: 120px;
            }
        }

        @media (max-width: 576px) {
            .hero-content h1 {
                font-size: 2.2rem;
            }

            .form-row, .academy-meta, .hero-stats {
                grid-template-columns: 1fr;
            }

            .section-title {
                font-size: 2.2rem;
            }

            .about-gallery-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <!-- PRELOADER -->
    <div id="loader">
        <div class="loader-ring"></div>
        <div class="loader-text">MEMELISTIC EMPIRE</div>
    </div>

    <!-- HEADER / NAVIGATION -->
    <header id="header">
        <div class="nav-container">
            <a href="#" class="logo">MEMELISTIC <span>EMPIRE</span></a>
            <div class="menu-toggle" id="menuToggle">
                <i class="fas fa-bars"></i>
            </div>
            <nav class="nav-links" id="navLinks">
                <a href="#about">About</a>
                <a href="#services">Services</a>
                <a href="#gallery">Wig Collection</a>
                <a href="#academy">Training Academy</a>
                <a href="#why-us">Why Us</a>
                <a href="#booking">Bookings</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="hero-container">
            <div class="hero-content">
                <h1>Luxury Wig Making, Installation & Training <span>in Lagos</span></h1>
                <p>We give your wigs a second chance through professional revamping, installation, styling, and premium machine wig making.</p>
                
                <div class="hero-cta">
                    <a href="#academy-register" class="btn-gold"><i class="fas fa-graduation-cap"></i> Register For Training</a>
                    <a href="#booking" class="btn-outline"><i class="fas fa-calendar-alt"></i> Book Appointment</a>
                </div>

                <div class="hero-stats">
                    <div class="stat-badge glass-card">
                        <i class="fas fa-user-graduate"></i>
                        <span>200+ Students Trained</span>
                    </div>
                    <div class="stat-badge glass-card">
                        <i class="fas fa-crown"></i>
                        <span>Luxury Wig Specialist</span>
                    </div>
                    <div class="stat-badge glass-card">
                        <i class="fas fa-award"></i>
                        <span>Professional Wig Trainer</span>
                    </div>
                    <div class="stat-badge glass-card">
                        <i class="fas fa-map-marker-alt"></i>
                        <span>Lagos, Nigeria</span>
                    </div>
                </div>
            </div>

            <div class="hero-image-wrapper">
                <img src="https://i.ibb.co/qLddXYBK/Screenshot-20260727-094548-Instagram-Lite.jpg" alt="Memelistic Empire Founder" class="hero-img-main">
                <div class="floating-card glass-card">
                    <div style="font-weight: 700; color: var(--soft-brown); font-size: 1.1rem;">Excellence Defined</div>
                    <div style="font-size: 0.85rem; color: var(--elegant-grey);">Crafting bespoke luxury wigs with master precision.</div>
                </div>
            </div>
        </div>
    </section>

    <!-- ABOUT SECTION -->
    <section class="about-section" id="about">
        <div class="about-container">
            <div class="about-gallery-grid">
                <img src="https://i.ibb.co/Y4j8s81F/1785106068277.png" alt="Memelistic Wig Styling" class="about-img">
                <img src="https://i.ibb.co/6JHyGg2P/images-13-7.jpg" alt="Memelistic Salon Service" class="about-img" style="margin-top: 30px;">
                <img src="https://i.ibb.co/SXLnxMzJ/Screenshot-20260726-234631-Google.jpg" alt="Wig Installation" class="about-img">
                <img src="https://i.ibb.co/RpBc9GVZ/Screenshot-20260726-234924-Google.jpg" alt="Academy Class" class="about-img" style="margin-top: 30px;">
            </div>

            <div class="about-content">
                <span class="section-subtitle">Welcome to Elegance</span>
                <h2>Redefining Hair Luxury & Professional Education</h2>
                <p>At <strong>Memelistic Empire</strong>, we believe every woman deserves flawless, effortless beauty. Operating from the heart of Lagos, we specialize in high-end wig artistry, precision styling, and transforming raw extensions into crown-worthy masterpieces.</p>
                <p>Our Academy is dedicated to raising the next generation of beauty entrepreneurs with world-class, hands-on wig making and styling skills.</p>
                
                <div class="services-tags">
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Luxury Wig Sales</span>
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Wig Revamping</span>
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Glueless Installation</span>
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Machine Wig Making</span>
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Custom Colouring</span>
                    <span class="tag"><i class="fas fa-check-circle" style="color:var(--champagne-gold);"></i> Lace Customization</span>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section class="services-section" id="services">
        <div class="section-header">
            <span class="section-subtitle">Our Expertise</span>
            <h2 class="section-title">Bespoke Hair Services</h2>
        </div>

        <div class="services-grid">
            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-cog"></i></div>
                <h3>Machine Wig Making</h3>
                <p>Durable, neat, and perfectly fitted machine-sewn wigs designed to match your exact head measurements.</p>
            </div>

            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-cut"></i></div>
                <h3>Professional Installation</h3>
                <p>Flawless glueless and lace melt installations for a natural hairline look without damage to your edges.</p>
            </div>

            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-magic"></i></div>
                <h3>Luxury Wig Styling</h3>
                <p>From Hollywood waves to sleek bobs and reverse bounce curls—masterfully styled to turn heads.</p>
            </div>

            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-sync-alt"></i></div>
                <h3>Hair Revamping</h3>
                <p>Restore life, shine, and soft texture to old, tangled, or dull wigs with our deep conditioning treatments.</p>
            </div>

            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-palette"></i></div>
                <h3>Hair Colouring</h3>
                <p>Custom dyeing, highlights, balayage, and pastel tones done safely without compromising hair quality.</p>
            </div>

            <div class="service-card glass-card">
                <div class="service-icon"><i class="fas fa-crown"></i></div>
                <h3>Lace Customization</h3>
                <p>Bleaching knots, plucking, and tinting frontals or closures to seamlessly match your unique skin tone.</p>
            </div>
        </div>
    </section>

    <!-- WIG GALLERY SECTION -->
    <section class="wig-gallery-section" id="gallery">
        <div class="section-header">
            <span class="section-subtitle">The Luxe Collection</span>
            <h2 class="section-title">Signature Wig Gallery</h2>
        </div>

        <div class="gallery-grid">
            <!-- Wig Item 1 -->
            <div class="wig-card">
                <div class="wig-img-box">
                    <img src="https://i.ibb.co/Y4j8s81F/1785106068277.png" alt="Luxury Body Wave Wig">
                </div>
                <div class="wig-info">
                    <h4>Signature Body Wave</h4>
                    <div class="wig-actions">
                        <button class="btn-outline btn-sm preview-btn" data-img="https://i.ibb.co/Y4j8s81F/1785106068277.png">View Details</button>
                        <a href="https://wa.me/2348143428822?text=Hello%20Memelistic%20Empire,%20I%20am%20interested%20in%20the%20Signature%20Body%20Wave%20Wig." target="_blank" class="btn-gold btn-sm"><i class="fab fa-whatsapp"></i> Enquire</a>
                    </div>
                </div>
            </div>

            <!-- Wig Item 2 -->
            <div class="wig-card">
                <div class="wig-img-box">
                    <img src="https://i.ibb.co/6JHyGg2P/images-13-7.jpg" alt="Silky Straight Frontal Wig">
                </div>
                <div class="wig-info">
                    <h4>Bone Straight Luxe</h4>
                    <div class="wig-actions">
                        <button class="btn-outline btn-sm preview-btn" data-img="https://i.ibb.co/6JHyGg2P/images-13-7.jpg">View Details</button>
                        <a href="https://wa.me/2348143428822?text=Hello%20Memelistic%20Empire,%20I%20am%20interested%20in%20the%20Bone%20Straight%20Luxe%20Wig." target="_blank" class="btn-gold btn-sm"><i class="fab fa-whatsapp"></i> Enquire</a>
                    </div>
                </div>
            </div>

            <!-- Wig Item 3 -->
            <div class="wig-card">
                <div class="wig-img-box">
                    <img src="https://i.ibb.co/SXLnxMzJ/Screenshot-20260726-234631-Google.jpg" alt="Custom Colored Bob Wig">
                </div>
                <div class="wig-info">
                    <h4>Honey Blonde Bob</h4>
                    <div class="wig-actions">
                        <button class="btn-outline btn-sm preview-btn" data-img="https://i.ibb.co/SXLnxMzJ/Screenshot-20260726-234631-Google.jpg">View Details</button>
                        <a href="https://wa.me/2348143428822?text=Hello%20Memelistic%20Empire,%20I%20am%20interested%20in%20the%20Honey%20Blonde%20Bob%20Wig." target="_blank" class="btn-gold btn-sm"><i class="fab fa-whatsapp"></i> Enquire</a>
                    </div>
                </div>
            </div>

            <!-- Wig Item 4 -->
            <div class="wig-card">
                <div class="wig-img-box">
                    <img src="https://i.ibb.co/RpBc9GVZ/Screenshot-20260726-234924-Google.jpg" alt="Deep Curls Glueless Wig">
                </div>
                <div class="wig-info">
                    <h4>Exotic Water Curls</h4>
                    <div class="wig-actions">
                        <button class="btn-outline btn-sm preview-btn" data-img="https://i.ibb.co/RpBc9GVZ/Screenshot-20260726-234924-Google.jpg">View Details</button>
                        <a href="https://wa.me/2348143428822?text=Hello%20Memelistic%20Empire,%20I%20am%20interested%20in%20the%20Exotic%20Water%20Curls%20Wig." target="_blank" class="btn-gold btn-sm"><i class="fab fa-whatsapp"></i> Enquire</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- TRAINING ACADEMY SECTION -->
    <section class="academy-section" id="academy">
        <div class="section-header">
            <span class="section-subtitle">Empowerment & Excellence</span>
            <h2 class="section-title">Become a Professional Wig Maker</h2>
        </div>

        <div class="academy-banner glass-card">
            <div class="academy-details">
                <h3>6 Weeks Professional Wig Making & Styling Masterclass</h3>
                <p style="margin-bottom: 20px; color: var(--elegant-grey);">Designed for beginners, intermediate stylists, and professionals looking to upgrade their skills to luxury industry standards.</p>
                
                <div class="price-badge">
                    <span>Training Fee: </span><span class="amount">₦400,000</span>
                    <div style="font-size:0.8rem; color:var(--text-dark);">Registration Fee: ₦5,000</div>
                </div>

                <div class="academy-meta">
                    <div class="meta-item"><i class="fas fa-calendar-alt"></i> Monday – Thursday</div>
                    <div class="meta-item"><i class="fas fa-clock"></i> 10:00 AM – 1:00 PM</div>
                    <div class="meta-item"><i class="fas fa-certificate"></i> Certificate Awarded</div>
                    <div class="meta-item"><i class="fas fa-bed"></i> Accommodation Available</div>
                </div>

                <a href="#academy-register" class="btn-gold"><i class="fas fa-user-plus"></i> Enroll Now (Limited Slots)</a>
            </div>

            <div>
                <img src="https://i.ibb.co/m5PV220Y/Screenshot-20260726-235051-Google.jpg" alt="Wig Training Masterclass" style="border-radius: 20px; width:100%;">
            </div>
        </div>

        <div class="section-header" style="margin-bottom: 30px;">
            <h3 class="serif-font" style="font-size: 2rem; color: var(--soft-brown);">What Students Will Learn</h3>
        </div>

        <div class="curriculum-grid">
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Glueless Wig Construction</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Machine Wig Making</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Professional Installation</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Wig Revamping Techniques</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Advanced Wig Styling</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Hair Layering & Cutting</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Lace Customization & Bleaching</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Professional Hair Colouring</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Heatless Curl Creation</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Water Curl Definition</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Reverse Bounce Styling</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Bang & Bob Precision Styling</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Wig Packaging Guide</div>
            <div class="curriculum-item glass-card"><i class="fas fa-check-circle"></i> Basic Starter Kit Included</div>
        </div>
    </section>

    <!-- TESTIMONIALS SECTION -->
    <section class="testimonials-section">
        <div class="section-header">
            <span class="section-subtitle">Student Success</span>
            <h2 class="section-title">Graduates & Reviews</h2>
        </div>

        <div class="slider-container">
            <div class="testimonial-track" id="testimonialTrack">
                <!-- Slide 1 -->
                <div class="testimonial-slide">
                    <img src="https://i.ibb.co/Q7MYMG1F/Screenshot-20260726-235202-Google.jpg" alt="Graduate Testimonial" class="student-avatar">
                    <p class="testimonial-text">"Training at Memelistic Empire changed my wig making career completely. I learned machine wig stitching with absolute confidence. I earned back my full tuition within 2 months of graduating!"</p>
                    <div class="student-name">Adesewa O.</div>
                    <div style="font-size: 0.85rem; color: var(--champagne-gold);">Lagos Graduate</div>
                </div>

                <!-- Slide 2 -->
                <div class="testimonial-slide">
                    <img src="https://i.ibb.co/m5PV220Y/Screenshot-20260726-235051-Google.jpg" alt="Graduate Review" class="student-avatar">
                    <p class="testimonial-text">"The detailed breakdown of lace tinting and color mixing is unmatched. The practical hands-on experience gave me immediate confidence to launch my own brand."</p>
                    <div class="student-name">Blessing E.</div>
                    <div style="font-size: 0.85rem; color: var(--champagne-gold);">Online Student</div>
                </div>
            </div>

            <div class="slider-controls">
                <button class="slider-btn" id="prevSlide"><i class="fas fa-chevron-left"></i></button>
                <button class="slider-btn" id="nextSlide"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
    </section>

    <!-- WHY CHOOSE US -->
    <section class="why-us-section" id="why-us">
        <div class="section-header">
            <span class="section-subtitle">The Gold Standard</span>
            <h2 class="section-title">Why Choose Memelistic Empire</h2>
        </div>

        <div class="why-grid">
            <div class="why-card glass-card">
                <i class="fas fa-chalkboard-teacher"></i>
                <h4>Professional Trainers</h4>
                <p>Guided step-by-step by master stylists active in the industry.</p>
            </div>

            <div class="why-card glass-card">
                <i class="fas fa-spa"></i>
                <h4>Luxury Environment</h4>
                <p>Learn and get styled in a modern, ultra-comfortable studio environment.</p>
            </div>

            <div class="why-card glass-card">
                <i class="fas fa-hands-helping"></i>
                <h4>Hands-on Practical</h4>
                <p>100% practical training using state-of-the-art machines and real wigs.</p>
            </div>

            <div class="why-card glass-card">
                <i class="fas fa-certificate"></i>
                <h4>Certification</h4>
                <p>Recognized professional certification upon course completion.</p>
            </div>

            <div class="why-card glass-card">
                <i class="fas fa-briefcase"></i>
                <h4>Business Mentorship</h4>
                <p>We teach you branding, client acquisition, and wig pricing strategies.</p>
            </div>

            <div class="why-card glass-card">
                <i class="fas fa-headset"></i>
                <h4>Student Support</h4>
                <p>Lifetime access to mentorship groups and continuous updates.</p>
            </div>
        </div>
    </section>

    <!-- MASONRY GALLERY -->
    <section class="masonry-section">
        <div class="section-header">
            <span class="section-subtitle">Moments & Creations</span>
            <h2 class="section-title">Life at The Empire</h2>
        </div>

        <div class="masonry-grid">
            <div class="masonry-item">
                <img src="https://i.ibb.co/Y4j8s81F/1785106068277.png" alt="Wig Creation">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
            <div class="masonry-item">
                <img src="https://i.ibb.co/6JHyGg2P/images-13-7.jpg" alt="Salon Life">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
            <div class="masonry-item">
                <img src="https://i.ibb.co/SXLnxMzJ/Screenshot-20260726-234631-Google.jpg" alt="Student Class">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
            <div class="masonry-item">
                <img src="https://i.ibb.co/RpBc9GVZ/Screenshot-20260726-234924-Google.jpg" alt="Graduate Moment">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
            <div class="masonry-item">
                <img src="https://i.ibb.co/m5PV220Y/Screenshot-20260726-235051-Google.jpg" alt="Styling Class">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
            <div class="masonry-item">
                <img src="https://i.ibb.co/Q7MYMG1F/Screenshot-20260726-235202-Google.jpg" alt="Student Certificate">
                <div class="masonry-overlay"><i class="fas fa-search-plus"></i></div>
            </div>
        </div>
    </section>

    <!-- FORMS SECTION (TRAINING & APPOINTMENT) -->
    <section class="forms-container-section" id="booking">
        <div class="forms-wrapper">
            <!-- Training Registration Form -->
            <div class="form-box" id="academy-register">
                <h3>Academy Registration</h3>
                <form id="trainingForm">
                    <div class="form-group">
                        <label>Full Name</label>
                        <input type="text" class="form-control" required placeholder="Jane Doe">
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label>Phone Number</label>
                            <input type="tel" class="form-control" required placeholder="+234 ...">
                        </div>
                        <div class="form-group">
                            <label>Email Address</label>
                            <input type="email" class="form-control" required placeholder="jane@example.com">
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label>Gender</label>
                            <select class="form-control">
                                <option>Female</option>
                                <option>Male</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label>Age</label>
                            <input type="number" class="form-control" placeholder="24">
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label>State</label>
                            <input type="text" class="form-control" placeholder="Lagos">
                        </div>
                        <div class="form-group">
                            <label>Country</label>
                            <input type="text" class="form-control" value="Nigeria">
                        </div>
                    </div>

                    <div class="form-group">
                        <label>Training Type</label>
                        <select class="form-control">
                            <option>Physical Training</option>
                            <option>Online Training</option>
                        </select>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label>Accommodation Needed?</label>
                            <select class="form-control">
                                <option>No</option>
                                <option>Yes</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label>Experience Level</label>
                            <select class="form-control">
                                <option>Beginner</option>
                                <option>Intermediate</option>
                                <option>Advanced</option>
                            </select>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>Preferred Start Date</label>
                        <input type="date" class="form-control">
                    </div>

                    <div class="form-group">
                        <label>Message / Note</label>
                        <textarea class="form-control" rows="3" placeholder="Any special requests?"></textarea>
                    </div>

                    <button type="submit" class="btn-gold" style="width: 100%; justify-content: center;">Submit Registration</button>
                </form>
            </div>

            <!-- Appointment Booking Form -->
            <div class="form-box">
                <h3>Book Salon Appointment</h3>
                <form id="appointmentForm">
                    <div class="form-group">
                        <label>Full Name</label>
                        <input type="text" class="form-control" required placeholder="Queen Smith">
                    </div>

                    <div class="form-group">
                        <label>Phone Number</label>
                        <input type="tel" class="form-control" required placeholder="+234 ...">
                    </div>

                    <div class="form-group">
                        <label>Service Needed</label>
                        <select class="form-control">
                            <option>Glueless Wig Installation</option>
                            <option>Wig Revamping & Treatment</option>
                            <option>Machine Wig Making</option>
                            <option>Lace Customization & Tint</option>
                            <option>Hair Colouring</option>
                            <option>Consultation</option>
                        </select>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label>Preferred Date</label>
                            <input type="date" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label>Preferred Time</label>
                            <input type="time" class="form-control" required>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>Additional Notes</label>
                        <textarea class="form-control" rows="4" placeholder="Describe hair length or wig state..."></textarea>
                    </div>

                    <button type="submit" class="btn-gold" style="width: 100%; justify-content: center;">Confirm Appointment</button>
                </form>
            </div>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="faq-section">
        <div class="section-header">
            <span class="section-subtitle">Clarification</span>
            <h2 class="section-title">Frequently Asked Questions</h2>
        </div>

        <div class="faq-accordion">
            <div class="faq-item">
                <div class="faq-header">How long is the wig masterclass training? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">The training program runs for 6 intensive weeks, combining both theoretical guidance and intensive practical sessions.</div>
            </div>

            <div class="faq-item">
                <div class="faq-header">Do I receive an official certificate? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Yes, upon successful completion and practical evaluation, every student is awarded an official Certificate of Completion from Memelistic Empire Academy.</div>
            </div>

            <div class="faq-item">
                <div class="faq-header">Can complete beginners apply? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Yes! Our course is specifically built from scratch. We teach fundamental concepts before advancing to expert machine wig making and styling.</div>
            </div>

            <div class="faq-item">
                <div class="faq-header">Is accommodation available for out-of-state students? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Yes, safe and comfortable accommodation options are available upon early request for students traveling from outside Lagos.</div>
            </div>

            <div class="faq-item">
                <div class="faq-header">Do you offer online classes? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Yes, we have a structured Online Training Masterclass with detailed videos and active interactive support.</div>
            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section class="contact-section" id="contact">
        <div class="contact-grid">
            <div class="contact-info">
                <div>
                    <span class="section-subtitle">Reach Us</span>
                    <h2 class="serif-font" style="font-size: 2.5rem; color: var(--soft-brown);">Get In Touch</h2>
                </div>

                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <div>
                        <h4 style="color:var(--soft-brown);">Salon Location</h4>
                        <p style="color:var(--elegant-grey);">37 Ayobo Road, Oluwaga Bus Stop, beside Peridot Filling Station, Lagos, Nigeria.</p>
                    </div>
                </div>

                <div class="contact-item">
                    <i class="fas fa-phone-alt"></i>
                    <div>
                        <h4 style="color:var(--soft-brown);">Direct Call / WhatsApp</h4>
                        <p style="color:var(--elegant-grey);">+234 814 342 8822</p>
                    </div>
                </div>

                <div class="contact-item">
                    <i class="fab fa-instagram"></i>
                    <div>
                        <h4 style="color:var(--soft-brown);">Instagram Pages</h4>
                        <p style="color:var(--elegant-grey);">Brand: <strong>@memelistic_hairplace</strong><br>Academy: <strong>@memelistic_hair_academy</strong></p>
                    </div>
                </div>
            </div>

            <div class="map-box">
                <!-- Embedded Google Maps Placeholder Location -->
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3963.155735235282!2d3.2505!3d6.6275!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNsKwMzcnNDEuMCJOIDPCsDE1JzAxLjgiRQ!5e0!3m2!1sen!2sng!4v1620000000000!5m2!1sen!2sng" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="footer-container">
            <div>
                <div class="footer-logo">MEMELISTIC EMPIRE</div>
                <p style="color: var(--warm-nude); font-size: 0.9rem;">The premier luxury wig destination and academy in Lagos, Nigeria. Restoring beauty and giving wigs a premium touch.</p>
                <div class="social-icons">
                    <a href="https://instagram.com/memelistic_hairplace" target="_blank"><i class="fab fa-instagram"></i></a>
                    <a href="https://wa.me/2348143428822" target="_blank"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>

            <div class="footer-links">
                <h5>Quick Links</h5>
                <ul>
                    <li><a href="#about">About Empire</a></li>
                    <li><a href="#services">Our Services</a></li>
                    <li><a href="#gallery">Wig Collection</a></li>
                    <li><a href="#academy">Training Academy</a></li>
                </ul>
            </div>

            <div class="footer-links">
                <h5>Services</h5>
                <ul>
                    <li><a href="#booking">Wig Installation</a></li>
                    <li><a href="#booking">Hair Revamping</a></li>
                    <li><a href="#booking">Machine Wig Making</a></li>
                    <li><a href="#booking">Custom Colouring</a></li>
                </ul>
            </div>

            <div>
                <h5 style="color: var(--champagne-gold); margin-bottom: 20px;">Studio Hours</h5>
                <p style="color: var(--warm-nude); font-size:0.9rem;">Monday - Saturday: 9:00 AM - 6:00 PM</p>
                <p style="color: var(--warm-nude); font-size:0.9rem; margin-top: 10px;">Sunday: Strictly By Appointment</p>
            </div>
        </div>

        <div class="copyright">
            &copy; 2026 Memelistic Empire. All Rights Reserved. Crafted with Luxury.
        </div>
    </footer>

    <!-- FLOATING ELEMENTS -->
    <a href="https://wa.me/2348143428822?text=Hello%20Memelistic%20Empire,%20I%20want%20to%20make%20an%20enquiry." class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <div class="back-to-top" id="backToTop">
        <i class="fas fa-chevron-up"></i>
    </div>

    <!-- LIGHTBOX MODAL -->
    <div class="lightbox-modal" id="lightbox">
        <span class="lightbox-close" id="lightboxClose">&times;</span>
        <img class="lightbox-content" id="lightboxImg" src="" alt="Preview">
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // --- 1. PRELOADER ---
        window.addEventListener('load', () => {
            const loader = document.getElementById('loader');
            loader.style.opacity = '0';
            setTimeout(() => {
                loader.style.display = 'none';
            }, 600);
        });

        // --- 2. HEADER STICKY & MOBILE NAV ---
        const header = document.getElementById('header');
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');

        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        // Close nav on click link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });

        // --- 3. TESTIMONIAL SLIDER ---
        const track = document.getElementById('testimonialTrack');
        const prevBtn = document.getElementById('prevSlide');
        const nextBtn = document.getElementById('nextSlide');
        let currentSlide = 0;
        const totalSlides = document.querySelectorAll('.testimonial-slide').length;

        function updateSlider() {
            track.style.transform = `translateX(-${currentSlide * 100}%)`;
        }

        nextBtn.addEventListener('click', () => {
            currentSlide = (currentSlide + 1) % totalSlides;
            updateSlider();
        });

        prevBtn.addEventListener('click', () => {
            currentSlide = (currentSlide - 1 + totalSlides) % totalSlides;
            updateSlider();
        });

        // --- 4. FAQ ACCORDION ---
        const faqItems = document.querySelectorAll('.faq-item');
        faqItems.forEach(item => {
            const header = item.querySelector('.faq-header');
            header.addEventListener('click', () => {
                faqItems.forEach(i => {
                    if (i !== item) i.classList.remove('active');
                });
                item.classList.toggle('active');
            });
        });

        // --- 5. LIGHTBOX FUNCTIONALITY ---
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = document.getElementById('lightboxImg');
        const lightboxClose = document.getElementById('lightboxClose');

        document.querySelectorAll('.preview-btn, .masonry-item').forEach(element => {
            element.addEventListener('click', (e) => {
                let src = '';
                if (element.classList.contains('preview-btn')) {
                    src = element.getAttribute('data-img');
                } else if (element.classList.contains('masonry-item')) {
                    src = element.querySelector('img').src;
                }
                lightboxImg.src = src;
                lightbox.style.display = 'flex';
            });
        });

        lightboxClose.addEventListener('click', () => {
            lightbox.style.display = 'none';
        });

        lightbox.addEventListener('click', (e) => {
            if (e.target === lightbox) {
                lightbox.style.display = 'none';
            }
        });

        // --- 6. BACK TO TOP BUTTON ---
        const backToTop = document.getElementById('backToTop');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 400) {
                backToTop.classList.add('show');
            } else {
                backToTop.classList.remove('show');
            }
        });

        backToTop.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });

        // --- 7. FORM SUBMISSIONS ---
        document.getElementById('trainingForm').addEventListener('submit', (e) => {
            e.preventDefault();
            alert("Thank you for registering. We will contact you shortly.");
            e.target.reset();
        });

        document.getElementById('appointmentForm').addEventListener('submit', (e) => {
            e.preventDefault();
            alert("Thank you for booking an appointment. Our team will contact you shortly to confirm your schedule.");
            e.target.reset();
        });
    </script>
</body>
</html>
