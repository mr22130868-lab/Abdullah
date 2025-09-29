<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مؤسسة دبي الإنشائية | البناء بمعايير الجودة</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* (CSS code as provided in your prompt) */
        :root {
            --primary-color: #2e7d32;
            --primary-dark: #1b5e20;
            --primary-light: #4caf50;
            --accent-color: #8bc34a;
            --text-color: #333;
            --light-bg: #c8f9b4;
            --white: #ffffff;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tajawal', 'Cairo', sans-serif;
        }
        body {
            background-color: var(--light-bg);
            color: var(--text-color);
            line-height: 1.6;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        .logo {
            display: flex;
            align-items: center;
        }
        .logo h1 {
            color: var(--primary-color);
            font-size: 1.8rem;
            margin-right: 10px;
        }
        .logo span {
            color: var(--primary-dark);
            font-weight: bold;
        }
        nav ul {
            display: flex;
            list-style: none;
        }
        nav ul li {
            margin-left: 25px;
        }
        nav ul li a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.3s;
            position: relative;
        }
        nav ul li a:hover {
            color: var(--primary-color);
        }
        nav ul li a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            right: 0;
            background-color: var(--primary-color);
            transition: width 0.3s;
        }
        nav ul li a:hover::after {
            width: 100%;
        }
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1541888946425-d81bb19240f5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80');
            background-size: cover;
            background-position: center;
            color: var(--white);
            text-align: center;
            padding: 120px 0;
            margin-bottom: 50px;
        }
        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        .cta-button {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--white);
            padding: 12px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
            margin: 0 10px;
        }
        .cta-button:hover {
            background-color: var(--primary-dark);
        }
        .about {
            padding: 80px 0;
            background-color: var(--white);
        }
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary-color);
            display: inline-block;
        }
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 3px;
            background-color: var(--primary-color);
            bottom: -10px;
            right: 50%;
            transform: translateX(50%);
        }
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        .about-text {
            flex: 1;
        }
        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--primary-dark);
        }
        .about-text p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s;
        }
        .about-image:hover img {
            transform: scale(1.05);
        }
        .services {
            padding: 80px 0;
            background-color: var(--light-bg);
        }
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        .service-card {
            background-color: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        .service-image {
            height: 200px;
            overflow: hidden;
        }
        .service-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        .service-card:hover .service-image img {
            transform: scale(1.1);
        }
        .service-content {
            padding: 20px;
        }
        .service-content h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        .projects {
            padding: 80px 0;
            background-color: var(--white);
        }
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        .project-card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        .project-image {
            height: 250px;
            overflow: hidden;
        }
        .project-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        .project-card:hover .project-image img {
            transform: scale(1.1);
        }
        .project-overlay {
            position: absolute;
            bottom: 0;
            right: 0;
            left: 0;
            background: linear-gradient(transparent, rgba(46, 125, 50, 0.9));
            color: var(--white);
            padding: 20px;
            transform: translateY(100%);
            transition: transform 0.3s;
        }
        .project-card:hover .project-overlay {
            transform: translateY(0);
        }
        .project-overlay h3 {
            margin-bottom: 10px;
        }
        .contact {
            padding: 80px 0;
            background-color: var(--light-bg);
        }
        .contact-container {
            display: flex;
            gap: 40px;
        }
        .contact-info {
            flex: 1;
        }
        .contact-info h3 {
            color: var(--primary-color);
            margin-bottom: 20px;
            font-size: 1.8rem;
        }
        .contact-info p {
            margin-bottom: 30px;
            font-size: 1.1rem;
        }
        .contact-methods {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }
        .contact-method {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        .contact-icon {
            width: 50px;
            height: 50px;
            background-color: var(--primary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            font-size: 1.2rem;
        }
        .contact-details h4 {
            margin-bottom: 5px;
            color: var(--primary-dark);
        }
        .contact-buttons {
            display: flex;
            gap: 15px;
            margin-top: 30px;
        }
        .contact-btn {
            display: flex;
            align-items: center;
            gap: 10px;
            background-color: var(--primary-color);
            color: var(--white);
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        .contact-btn:hover {
            background-color: var(--primary-dark);
        }
        .whatsapp-btn {
            background-color: #25D366;
        }
        .whatsapp-btn:hover {
            background-color: #128C7E;
        }
        .contact-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        .contact-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        footer {
            background-color: var(--primary-dark);
            color: var(--white);
            padding: 40px 0 20px;
        }
        .footer-container {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 30px;
        }
        .footer-col {
            flex: 1;
            min-width: 250px;
        }
        .footer-col h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        .footer-col h3::after {
            content: '';
            position: absolute;
            width: 50px;
            height: 2px;
            background-color: var(--accent-color);
            bottom: 0;
            right: 0;
        }
        .footer-col p {
            margin-bottom: 20px;
        }
        .social-links {
            display: flex;
            gap: 15px;
        }
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: var(--white);
            text-decoration: none;
            transition: background-color 0.3s;
        }
        .social-links a:hover {
            background-color: var(--primary-color);
        }
        .footer-links {
            list-style: none;
        }
        .footer-links li {
            margin-bottom: 10px;
        }
        .footer-links a {
            color: var(--white);
            text-decoration: none;
            transition: color 0.3s;
        }
        .footer-links a:hover {
            color: var(--accent-color);
        }
        .copyright {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        @media (max-width: 992px) {
            .about-content, .contact-container {
                flex-direction: column;
            }
            .hero h2 {
                font-size: 2.5rem;
            }
        }
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
            }
            nav ul {
                margin-top: 15px;
            }
            nav ul li {
                margin: 0 10px;
            }
            .hero h2 {
                font-size: 2rem;
            }
            .section-title h2 {
                font-size: 2rem;
            }
            .contact-buttons {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <h1>مؤسسة <span>دبي</span> الإنشائية</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">الرئيسية</a></li>
                    <li><a href="#about">من نحن</a></li>
                    <li><a href="#services">خدماتنا</a></li>
                    <li><a href="#projects">مشاريعنا</a></li>
                    <li><a href="#contact">اتصل بنا</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h2>بناء مستقبل أفضل مع مؤسسة دبي الإنشائية</h2>
            <p>نحن نقدم حلولاً إنشائية مبتكرة تلبي أعلى معايير الجودة والسلامة، مع الالتزام بمواعيد التسليم وتقديم أفضل الخدمات لعملائنا في المملكة العربية السعودية.</p>
            <a href="#contact" class="cta-button">اتصل بنا الآن</a>
            <a href="#projects" class="cta-button">شاهد مشاريعنا</a>
        </div>
    </section>
    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="section-title">
                <h2>من نحن</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>رواد في مجال الإنشاءات منذ أكثر من 15 عاماً</h3>
                    <p>مؤسسة دبي الإنشائية هي شركة رائدة في مجال المقاولات والإنشاءات، تأسست برؤية واضحة لتقديم حلول إنشائية متكاملة تلبي احتياجات العملاء في مختلف القطاعات.</p>
                    <p>نتميز بفريق من المهندسين والمختصين ذوي الخبرة الواسعة، ونستخدم أحدث التقنيات والمواد لضمان جودة المشاريع التي ننفذها.</p>
                    <p>نسعى دائماً للتميز والريادة في مجال الإنشاءات من خلال الالتزام بمعايير الجودة والسلامة وتقديم خدمات متميزة تلبي توقعات عملائنا.</p>
                </div>
                <div class="about-image">
                    <img src="wصور/f11ac857-c5bd-4d32-9298-1e576fcfe787.jpg" alt="مؤسسة دبي الإنشائية">
                </div>
            </div>
        </div>
    </section>
    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>خدماتنا</h2>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-image">
                        <img src="wصور/509e4957-644d-46f9-a992-edf522eebe35.jpg" alt="التصميم المعماري">
                    </div>
                    <div class="service-content">
                        <h3>التصميم المعماري والإنشائي</h3>
                        <p>نقدم حلول تصميم مبتكرة تلبي احتياجات العملاء الجمالية والوظيفية مع الالتزام بالمعايير الإنشائية والهندسية.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-image">
                        <img src="wصور/WhatsApp Image 2025-09-25 at 3.28.33 PM.jpeg" alt="إدارة المشاريع">
                    </div>
                    <div class="service-content">
                        <h3>إدارة المشاريع الإنشائية</h3>
                        <p>إدارة متكاملة للمشاريع الإنشائية من التخطيط حتى التسليم، مع الالتزام بالجودة والمواعيد والميزانية المحددة.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-image">
                        <img src="wصور/cb3ee625-451a-4bf9-ad90-9829ba71af01.jpg" alt="المقاولات العامة">
                    </div>
                    <div class="service-content">
                        <h3>المقاولات العامة</h3>
                        <p>تنفيذ المشاريع الإنشائية بكافة أنواعها من المباني السكنية والتجارية والمنشآت الصناعية والمرافق العامة.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Projects Section -->
    <section class="projects" id="projects">
        <div class="container">
            <div class="section-title">
                <h2>مشاريعنا</h2>
            </div>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1074&q=80" alt="مشروع سكني">
                    </div>
                    <div class="project-overlay">
                        <h3>مجمع سكني فاخر</h3>
                        <p>تصميم وتنفيذ مجمع سكني فاخر يتكون من 50 فيلا بتصاميم معاصرة.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="مشروع تجاري">
                    </div>
                    <div class="project-overlay">
                        <h3>مركز تجاري حديث</h3>
                        <p>بناء مركز تجاري متكامل بمساحة 20,000 متر مربع في قلب المدينة.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="مشروع صناعي">
                    </div>
                    <div class="project-overlay">
                        <h3>منشأة صناعية متطورة</h3>
                        <p>تصميم وتنفيذ منشأة صناعية بتقنيات متطورة لشركة رائدة في مجال الصناعة.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>اتصل بنا</h2>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>نحن هنا لخدمتكم</h3>
                    <p>لا تتردد في التواصل معنا للحصول على استشارة مجانية أو لمعرفة المزيد عن خدماتنا. فريقنا متاح دائماً لمساعدتكم في تحقيق رؤيتكم الإنشائية.</p>
                    <div class="contact-methods">
                        <div class="contact-method">
                            <div class="contact-icon">
                                <i class="fas fa-user"></i>
                            </div>
                            <div class="contact-details">
                                <h4>المسؤول</h4>
                                <p>عبدلله أبو قصي</p>
                            </div>
                        </div>
                        <div class="contact-method">
                            <div class="contact-icon">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div class="contact-details">
                                <h4>الهاتف</h4>
                                <p>+966 53 630 6584</p>
                            </div>
                        </div>
                    </div>
                    <div class="contact-buttons">
                        <a href="tel:+966536306584" class="contact-btn">
                            <i class="fas fa-phone"></i>
                            اتصل بنا الآن
                        </a>
                        <a href="https://wa.me/966536306584" class="contact-btn whatsapp-btn">
                            <i class="fab fa-whatsapp"></i>
                            راسلنا على واتساب
                        </a>
                    </div>
                </div>
                <div class="contact-image">
                    <img src="wصور/90b9c447-d018-4bf3-aba5-2ec0f32d1938.jpg" alt="اتصل بنا">
                </div>
            </div>
        </div>
    </section>
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <h3>مؤسسة دبي الإنشائية</h3>
                    <p>شركة رائدة في مجال الإنشاءات والمقاولات العامة، نقدم حلولاً إنشائية متكاملة تلبي أعلى معايير الجودة والسلامة.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                <div class="footer-col">
                    <h3>روابط سريعة</h3>
                    <ul class="footer-links">
                        <li><a href="#home">الرئيسية</a></li>
                        <li><a href="#about">من نحن</a></li>
                        <li><a href="#services">خدماتنا</a></li>
                        <li><a href="#projects">مشاريعنا</a></li>
                        <li><a href="#contact">اتصل بنا</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>خدماتنا</h3>
                    <ul class="footer-links">
                        <li><a href="#">التصميم المعماري</a></li>
                        <li><a href="#">إدارة المشاريع</a></li>
                        <li><a href="#">المقاولات العامة</a></li>
                        <li><a href="#">الاستشارات الهندسية</a></li>
                        <li><a href="#">التشطيبات الداخلية</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>جميع الحقوق محفوظة &copy; 2023 مؤسسة دبي الإنشائية</p>
            </div>
        </div>
    </footer>
    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        // Add active class to navigation links on scroll
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('nav ul li a');
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if(scrollY >= (sectionTop - 100)) {
                    current = section.getAttribute('id');
                }
            });
            navLinks.forEach(link => {
                link.classList.remove('active');
                if(link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
