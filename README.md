<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="description"
content="Vamsi Web Design - Modern responsive websites for businesses, students and individuals.">

<title>VAMSI WEB DESIGN | Professional Websites</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

:root{
    --primary:#2563eb;
    --primary-dark:#1d4ed8;
    --bg:#f5f7fb;
    --card:#ffffff;
    --text:#111827;
    --muted:#64748b;
    --dark:#0f172a;
    --border:#e2e8f0;
    --shadow:0 10px 30px rgba(0,0,0,.08);
}

body{
    font-family:Arial, sans-serif;
    background:var(--bg);
    color:var(--text);
    line-height:1.6;
    transition:.3s;
}

body.dark{
    --bg:#0f172a;
    --card:#1e293b;
    --text:#f8fafc;
    --muted:#cbd5e1;
    --border:#334155;
    --shadow:0 10px 30px rgba(0,0,0,.3);
}

/* LOADING */

#loader{
    position:fixed;
    inset:0;
    background:var(--dark);
    color:white;
    display:flex;
    justify-content:center;
    align-items:center;
    z-index:9999;
    font-size:24px;
    font-weight:bold;
}

/* HEADER */

header{
    background:linear-gradient(135deg,#111827,#2563eb);
    color:white;
    padding:70px 20px;
    text-align:center;
}

.logo{
    font-size:34px;
    font-weight:bold;
}

header p{
    margin-top:10px;
    color:#dbeafe;
}

/* NAV */

nav{
    position:sticky;
    top:0;
    z-index:1000;
    background:var(--card);
    border-bottom:1px solid var(--border);
    display:flex;
    justify-content:center;
    align-items:center;
    padding:12px;
}

.nav-links{
    display:flex;
    gap:8px;
    list-style:none;
}

.nav-links a{
    text-decoration:none;
    color:var(--text);
    padding:9px 12px;
    border-radius:8px;
    font-size:14px;
}

.nav-links a:hover{
    background:var(--primary);
    color:white;
}

.menu-btn{
    display:none;
    border:0;
    background:var(--primary);
    color:white;
    padding:10px 14px;
    border-radius:8px;
    font-size:20px;
}

/* COMMON */

section{
    padding:70px 20px;
}

.container{
    max-width:1100px;
    margin:auto;
}

.section-title{
    text-align:center;
    font-size:30px;
    margin-bottom:12px;
}

.section-subtitle{
    text-align:center;
    color:var(--muted);
    margin-bottom:35px;
}

.btn{
    display:inline-block;
    border:0;
    background:var(--primary);
    color:white;
    padding:12px 22px;
    border-radius:9px;
    text-decoration:none;
    cursor:pointer;
    margin:6px;
    transition:.3s;
}

.btn:hover{
    background:var(--primary-dark);
    transform:translateY(-2px);
}

.btn-outline{
    background:transparent;
    border:2px solid var(--primary);
    color:var(--primary);
}

body.dark .btn-outline{
    color:white;
}

/* HERO */

.hero{
    min-height:650px;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    background:var(--card);
}

.hero-content{
    max-width:800px;
}

.badge{
    display:inline-block;
    background:#dbeafe;
    color:#1d4ed8;
    padding:7px 14px;
    border-radius:30px;
    font-size:13px;
    margin-bottom:18px;
}

body.dark .badge{
    background:#1e3a8a;
    color:#dbeafe;
}

.hero h1{
    font-size:52px;
    line-height:1.15;
    margin-bottom:20px;
}

.hero h1 span{
    color:var(--primary);
}

.hero p{
    color:var(--muted);
    font-size:18px;
    max-width:650px;
    margin:auto;
}

/* STATS */

.stats{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
    margin-top:40px;
}

.stat{
    background:var(--card);
    padding:20px;
    border-radius:14px;
    box-shadow:var(--shadow);
}

.stat h3{
    color:var(--primary);
    font-size:28px;
}

/* ABOUT */

.about{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:35px;
    align-items:center;
}

.about-card{
    background:var(--card);
    padding:30px;
    border-radius:18px;
    box-shadow:var(--shadow);
}

.about-card h3{
    margin-bottom:12px;
}

.about-card p{
    color:var(--muted);
}

.skills{
    margin-top:20px;
}

.skill{
    margin:15px 0;
}

.skill-top{
    display:flex;
    justify-content:space-between;
}

.skill-bar{
    height:9px;
    background:#e2e8f0;
    border-radius:20px;
    overflow:hidden;
}

body.dark .skill-bar{
    background:#334155;
}

.skill-fill{
    height:100%;
    background:var(--primary);
    border-radius:20px;
}

/* CARDS */

.grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.card{
    background:var(--card);
    padding:28px 22px;
    border-radius:18px;
    box-shadow:var(--shadow);
    border:1px solid var(--border);
    transition:.3s;
}

.card:hover{
    transform:translateY(-7px);
}

.icon{
    font-size:38px;
    margin-bottom:15px;
}

.card h3{
    margin-bottom:10px;
}

.card p{
    color:var(--muted);
}

/* SEARCH */

.search-box{
    max-width:600px;
    margin:0 auto 30px;
}

.search-box input{
    width:100%;
    padding:15px;
    border:1px solid var(--border);
    border-radius:10px;
    background:var(--card);
    color:var(--text);
    font-size:16px;
}

/* PROJECT */

.project-image{
    height:170px;
    border-radius:12px;
    background:linear-gradient(135deg,#2563eb,#7c3aed);
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
    font-size:45px;
    margin-bottom:18px;
}

/* PRICING */

.price{
    font-size:35px;
    color:var(--primary);
    font-weight:bold;
    margin:15px 0;
}

.price small{
    color:var(--muted);
    font-size:14px;
    font-weight:normal;
}

.price-list{
    list-style:none;
    margin:20px 0;
}

.price-list li{
    margin:10px 0;
    color:var(--muted);
}

/* TESTIMONIAL */

.quote{
    font-size:16px;
    color:var(--muted);
    font-style:italic;
    margin-bottom:15px;
}

.stars{
    color:#f59e0b;
}

/* CONTACT */

.contact{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:25px;
}

.contact-info,
.contact-form{
    background:var(--card);
    padding:28px;
    border-radius:18px;
    box-shadow:var(--shadow);
}

.contact-info p{
    margin:15px 0;
    color:var(--muted);
}

input,
textarea,
select{
    width:100%;
    padding:13px;
    margin:8px 0;
    border:1px solid var(--border);
    border-radius:9px;
    background:var(--bg);
    color:var(--text);
    font-size:15px;
}

textarea{
    height:130px;
    resize:none;
}

/* SOCIAL */

.socials{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin-top:20px;
}

.socials a{
    text-decoration:none;
    padding:9px 14px;
    border-radius:8px;
    background:var(--bg);
    color:var(--text);
}

/* FOOTER */

footer{
    background:#111827;
    color:white;
    text-align:center;
    padding:35px 20px;
}

footer p{
    color:#cbd5e1;
    margin:7px;
}

/* FLOATING WHATSAPP */

.whatsapp{
    position:fixed;
    right:20px;
    bottom:20px;
    width:58px;
    height:58px;
    background:#25D366;
    color:white;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:27px;
    text-decoration:none;
    z-index:999;
    box-shadow:0 5px 20px rgba(0,0,0,.2);
}

/* TOP BUTTON */

#topBtn{
    position:fixed;
    right:20px;
    bottom:90px;
    width:45px;
    height:45px;
    border:0;
    border-radius:50%;
    background:var(--primary);
    color:white;
    cursor:pointer;
    display:none;
}

/* TOAST */

#toast{
    position:fixed;
    left:50%;
    bottom:30px;
    transform:translateX(-50%);
    background:#111827;
    color:white;
    padding:12px 20px;
    border-radius:10px;
    display:none;
    z-index:2000;
}

/* MOBILE */

@media(max-width:800px){

    .hero h1{
        font-size:38px;
    }

    .stats{
        grid-template-columns:repeat(2,1fr);
    }

    .about,
    .contact{
        grid-template-columns:1fr;
    }

    .grid{
        grid-template-columns:1fr 1fr;
    }

    .menu-btn{
        display:block;
        margin-left:auto;
    }

    .nav-links{
        display:none;
        position:absolute;
        top:60px;
        left:0;
        right:0;
        background:var(--card);
        flex-direction:column;
        padding:15px;
        box-shadow:var(--shadow);
    }

    .nav-links.show{
        display:flex;
    }

}

@media(max-width:550px){

    header{
        padding:45px 15px;
    }

    .logo{
        font-size:27px;
    }

    .hero{
        min-height:560px;
    }

    .hero h1{
        font-size:32px;
    }

    .hero p{
        font-size:16px;
    }

    section{
        padding:50px 15px;
    }

    .section-title{
        font-size:26px;
    }

    .stats{
        grid-template-columns:1fr 1fr;
    }

    .grid{
        grid-template-columns:1fr;
    }

    .btn{
        width:90%;
        max-width:300px;
    }

}

</style>
</head>

<body>

<!-- LOADER -->

<div id="loader">
    VAMSI WEB SOLUTIONS 🚀
</div>


<!-- HEADER -->

<header>

    <div class="logo">
        VAMSI WEB SOLUTIONS
    </div>

    <p>
        Modern Websites • Responsive Design • Digital Solutions
    </p>

</header>


<!-- NAVIGATION -->

<nav>

    <button class="menu-btn" onclick="toggleMenu()">
        ☰
    </button>

    <ul class="nav-links" id="navLinks">

        <li><a href="#home">Home</a></li>

        <li><a href="#about">About</a></li>

        <li><a href="#services">Services</a></li>

        <li><a href="#projects">Projects</a></li>

        <li><a href="#pricing">Pricing</a></li>

        <li><a href="#contact">Contact</a></li>

        <li>
            <a href="#" onclick="toggleDark();return false;">
                🌙
            </a>
        </li>

    </ul>

</nav>


<!-- HERO -->

<section class="hero" id="home">

    <div class="hero-content">

        <span class="badge">
            AVAILABLE FOR PROJECTS
        </span>

        <h1>
            I Create
            <span>Modern Websites</span>
            For Your Business
        </h1>

        <p>
            Professional, responsive and mobile-friendly
            websites for businesses, students, creators
            and individuals.
        </p>

        <div>

            <a href="#contact" class="btn">
                🚀 Start a Project
            </a>

            <a href="#projects" class="btn btn-outline">
                View My Work
            </a>

        </div>


        <div class="stats">

            <div class="stat">
                <h3>10+</h3>
                <p>Projects</p>
            </div>

            <div class="stat">
                <h3>5+</h3>
                <p>Services</p>
            </div>

            <div class="stat">
                <h3>100%</h3>
                <p>Responsive</p>
            </div>

            <div class="stat">
                <h3>24/7</h3>
                <p>Contact</p>
            </div>

        </div>

    </div>

</section>


<!-- ABOUT -->

<section id="about">

    <div class="container">

        <h2 class="section-title">
            About Me
        </h2>

        <p class="section-subtitle">
            Web Designer & Developer
        </p>


        <div class="about">

            <div class="about-card">

                <h3>Hi, I'm Vamsi Chowdari👋</h3>

                <p>
                    I create modern websites using HTML,
                    CSS and JavaScript. My focus is on
                    clean design, mobile responsiveness
                    and simple user experiences.
                </p>

                <br>

                <p>
                    I can create websites for small
                    businesses, students, professionals,
                    shops and personal brands.
                </p>

            </div>


            <div class="about-card">

                <h3>My Skills</h3>

                <div class="skills">

                    <div class="skill">

                        <div class="skill-top">
                            <span>HTML</span>
                            <span>90%</span>
                        </div>

                        <div class="skill-bar">
                            <div
                            class="skill-fill"
                            style="width:90%">
                            </div>
                        </div>

                    </div>


                    <div class="skill">

                        <div class="skill-top">
                            <span>CSS</span>
                            <span>85%</span>
                        </div>

                        <div class="skill-bar">
                            <div
                            class="skill-fill"
                            style="width:85%">
                            </div>
                        </div>

                    </div>


                    <div class="skill">

                        <div class="skill-top">
                            <span>JavaScript</span>
                            <span>75%</span>
                        </div>

                        <div class="skill-bar">
                            <div
                            class="skill-fill"
                            style="width:75%">
                            </div>
                        </div>

                    </div>


                    <div class="skill">

                        <div class="skill-top">
                            <span>Responsive Design</span>
                            <span>90%</span>
                        </div>

                        <div class="skill-bar">
                            <div
                            class="skill-fill"
                            style="width:90%">
                            </div>
                        </div>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- SERVICES -->

<section id="services">

    <div class="container">

        <h2 class="section-title">
            My Services
        </h2>

        <p class="section-subtitle">
            Website solutions for different needs
        </p>


        <div class="grid" id="serviceGrid">


            <div class="card service-card">

                <div class="icon">💼</div>

                <h3>Business Website</h3>

                <p>
                    Professional websites for shops,
                    companies and local businesses.
                </p>

            </div>


            <div class="card service-card">

                <div class="icon">👤</div>

                <h3>Portfolio Website</h3>

                <p>
                    Modern portfolio websites for
                    students and professionals.
                </p>

            </div>


            <div class="card service-card">

                <div class="icon">🚀</div>

                <h3>Landing Page</h3>

                <p>
                    Attractive landing pages for
                    products and services.
                </p>

            </div>


            <div class="card service-card">

                <div class="icon">🛋️</div>

                <h3>Online Shop</h3>

                <p>
                    Product showcase websites for
                    small businesses and shops.
                </p>

            </div>


            <div class="card service-card">

                <div class="icon">🎨</div>

                <h3>Website Redesign</h3>

                <p>
                    Modernizing old websites with
                    responsive design.
                </p>

            </div>


            <div class="card service-card">

                <div class="icon">🛠️</div>

                <h3>Maintenance</h3>

                <p>
                    Website content updates and
                    basic maintenance services.
                </p>

            </div>


        </div>

    </div>

</section>


<!-- PROJECTS -->

<section id="projects">

    <div class="container">

        <h2 class="section-title">
            My Projects
        </h2>

        <p class="section-subtitle">
            Some sample projects
        </p>


        <div class="search-box">

            <input
                type="text"
                id="projectSearch"
                placeholder="🔍 Search projects..."
                onkeyup="searchProjects()"
            >

        </div>


        <div class="grid" id="projectGrid">


            <div class="card project-card">

                <div class="project-image">
                    🛋️
                </div>

                <h3>Furniture Website</h3>

                <p>
                    Modern furniture shopping website
                    with product cards and responsive design.
                </p>

                <button
                    class="btn"
                    onclick="showToast('Furniture Mart project selected')">
                    View Project
                </button>

            </div>


            <div class="card project-card">

                <div class="project-image">
                    🍔
                </div>

                <h3>Restaurant Website</h3>

                <p>
                    Responsive restaurant website
                    with menu and contact sections.
                </p>

                <button
                    class="btn"
                    onclick="showToast('Restaurant project selected')">
                    View Project
                </button>

            </div>


            <div class="card project-card">

                <div class="project-image">
                    🏠
                </div>

                <h3>Real Estate Website</h3>

                <p>
                    Property showcase website for
                    real estate businesses.
                </p>

                <button
                    class="btn"
                    onclick="showToast('Real Estate project selected')">
                    View Project
                </button>

            </div>


            <div class="card project-card">

                <div class="project-image">
                    👨‍💻
                </div>

                <h3>Personal Portfolio</h3>

                <p>
                    Professional personal portfolio
                    website.
                </p>

                <button
                    class="btn"
                    onclick="showToast('Portfolio project selected')">
                    View Project
                </button>

            </div>


        </div>

    </div>

</section>


<!-- PRICING -->

<section id="pricing">

    <div class="container">

        <h2 class="section-title">
            Website Packages
        </h2>

        <p class="section-subtitle">
            Starting prices — customize based on project requirements
        </p>


        <div class="grid">


            <div class="card">

                <div class="icon">🌱</div>

                <h3>Starter</h3>

                <div class="price">
                    ₹999
                    <small>/starting</small>
                </div>

                <ul class="price-list">

                    <li>✔ 1 Page Website</li>

                    <li>✔ Mobile Responsive</li>

                    <li>✔ Contact Section</li>

                    <li>✔ Basic Design</li>

                </ul>

                <a
                    href="#contact"
                    class="btn">
                    Choose
                </a>

            </div>


            <div class="card">

                <div class="icon">🚀</div>

                <h3>Business</h3>

                <div class="price">
                    ₹2,499
                    <small>/starting</small>
                </div>

                <ul class="price-list">

                    <li>✔ Multi-section Website</li>

                    <li>✔ Responsive Design</li>

                    <li>✔ WhaatsApp Button</li>

                    <li>✔ Contact Form</li>

                    <li>✔ Basic Animations</li>

                </ul>

                <a
                    href="#contact"
                    class="btn">
                    Choose
                </a>

            </div>


            <div class="card">

                <div class="icon">💎</div>

                <h3>Professional</h3>

                <div class="price">
                    ₹4,999
                    <small>/starting</small>
                </div>

                <ul class="price-list">

                    <li>✔ Advanced Design</li>

                    <li>✔ Multiple Pages</li>

                    <li>✔ JavaScript Features</li>

                    <li>✔ SEO Basics</li>

                    <li>✔ Deployment Support</li>

                </ul>

                <a
                    href="#contact"
                    class="btn">
                    Choose
                </a>

            </div>


        </div>

    </div>

</section>


<!-- TESTIMONIALS -->

<section>

    <div class="container">

        <h2 class="section-title">
            Client Feedback
        </h2>

        <p class="section-subtitle">
            Sample testimonial layout
        </p>


        <div class="grid">


            <div class="card">

                <p class="quote">
                    "The website looks clean and works
                    well on mobile."
                </p>

                <strong>
                    — Tippani Keerthana
                </strong>

                <div class="stars">
                    ★★★★★
                </div>

            </div>


            <div class="card">

                <p class="quote">
                    "Simple design and easy navigation."
                </p>

                <strong>
                    — Tejeswari Chowdari
                </strong>

                <div class="stars">
                    ★★★★★
                </div>

            </div>


            <div class="card">

                <p class="quote">
                    "Professional presentation for our business."
                </p>

                <strong>
                    — Uma Mahesh Goud
                </strong>

                <div class="stars">
                    ★★★★★
                </div>

            </div>


        </div>

    </div>

</section>


<!-- CONTACT -->

<section id="contact">

    <div class="container">

        <h2 class="section-title">
            Start Your Project
        </h2>

        <p class="section-subtitle">
            Tell me what website you need
        </p>


        <div class="contact">


            <div class="contact-info">

                <h3>Let's Work Together 🤝</h3>

                <p>
                    📧 vamsichowdari17@gmail.com
                </p>

                <p>
                    📱 WhatsApp available
                </p>

                <p>
                    🌐 Website Design
                </p>

                <p>
                    📍 Hyderabad, Telangana
                </p>


                <div class="socials">

                    <a href="#">
                        Instagram
                    </a>

                    <a href="#">
                        YouTube
                    </a>

                    <a href="#">
                        GitHub
                    </a>

                </div>

            </div>


            <div class="contact-form">

                <form onsubmit="sendForm(event)">

                    <input
                        type="text"
                        id="name"
                        placeholder="Your Name"
                        required
                    >

                    <input
                        type="tel"
                        id="phone"
                        placeholder="Phone Number"
                        required
                    >

                    <input
                        type="email"
                        id="email"
                        placeholder="Email Address"
                        required
                    >


                    <select id="service" required>

                        <option value="">
                            Select Service
                        </option>

                        <option>
                            Business Website
                        </option>

                        <option>
                            Portfolio Website
                        </option>

                        <option>
                            Landing Page
                        </option>

                        <option>
                            Online Shop
                        </option>

                        <option>
                            Website Redesign
                        </option>

                    </select>


                    <textarea
                        id="message"
                        placeholder="Tell me about your project..."
                        required>
                    </textarea>


                    <button
                        type="submit"
                        class="btn">
                        📩 Send Enquiry
                    </button>

                </form>

            </div>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    <h3>
        VAMSI WEB DESIGN
    </h3>

    <p>
        Modern Websites • Responsive Design • Digital Solutions
    </p>

    <p>
        © 2026 Vamsi Web Solutions. All Rights Reserved.
    </p>

</footer>


<!-- WHATSAPP -->

<a
    class="whatsapp"
    href="https://wa.me/917815862581?text=Hi%20Vamsi%2C%20I%20need%20a%20website."
    target="_blank"
    title="Chat on WhatsApp">

    💬

</a>


<!-- BACK TO TOP -->

<button
    id="topBtn"
    onclick="window.scrollTo(0,0)">
    ↑
</button>


<!-- TOAST -->

<div id="toast">
    Done!
</div>


<script>

/* LOADER */

window.addEventListener("load", function(){

    setTimeout(function(){

        document.getElementById("loader").style.display =
        "none";

    },800);

});


/* MOBILE MENU */

function toggleMenu(){

    document
    .getElementById("navLinks")
    .classList
    .toggle("show");

}


/* CLOSE MENU AFTER CLICK */

document
.querySelectorAll(".nav-links a")
.forEach(function(link){

    link.addEventListener("click",function(){

        document
        .getElementById("navLinks")
        .classList
        .remove("show");

    });

});


/* DARK MODE */

function toggleDark(){

    document
    .body
    .classList
    .toggle("dark");


    if(document.body.classList.contains("dark")){

        localStorage.setItem("theme","dark");

    }else{

        localStorage.setItem("theme","light");

    }

}


/* LOAD THEME */

if(localStorage.getItem("theme") === "dark"){

    document.body.classList.add("dark");

}


/* PROJECT SEARCH */

function searchProjects(){

    let input =
    document
    .getElementById("projectSearch")
    .value
    .toLowerCase();


    let projects =
    document
    .querySelectorAll(".project-card");


    projects.forEach(function(project){

        let text =
        project.innerText.toLowerCase();


        if(text.includes(input)){

            project.style.display = "";

        }else{

            project.style.display = "none";

        }

    });

}


/* CONTACT FORM */

function sendForm(event){

    event.preventDefault();


    let name =
    document.getElementById("name").value;

    let phone =
    document.getElementById("phone").value;

    let email =
    document.getElementById("email").value;

    let service =
    document.getElementById("service").value;

    let message =
    document.getElementById("message").value;


    let subject =
    "New Website Enquiry - " + service;


    let body =
    "Name: " + name +
    "\nPhone: " + phone +
    "\nEmail: " + email +
    "\nService: " + service +
    "\n\nMessage:\n" + message;


    localStorage.setItem(
        "lastEnquiry",
        JSON.stringify({
            name:name,
            phone:phone,
            email:email,
            service:service,
            message:message
        })
    );


    window.location.href =
    "mailto:vamsichowdari17@gmail.com" +
    "?subject=" +
    encodeURIComponent(subject) +
    "&body=" +
    encodeURIComponent(body);

}


/* TOAST */

function showToast(message){

    let toast =
    document.getElementById("toast");


    toast.innerText = message;

    toast.style.display = "block";


    setTimeout(function(){

        toast.style.display = "none";

    },2500);

}


/* BACK TO TOP */

window.addEventListener("scroll",function(){

    let button =
    document.getElementById("topBtn");


    if(window.scrollY > 400){

        button.style.display = "block";

    }else{

        button.style.display = "none";

    }

});

</script>

</body>
</html>
