/* =========================
   GLOBAL
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "Inter", sans-serif;
    background: #0b0d10;
    color: #ffffff;
    line-height: 1.6;
}

a {
    color: inherit;
    text-decoration: none;
}

img {
    width: 100%;
    display: block;
}

.container {
    width: min(1120px, 90%);
    margin: auto;
}

.section {
    padding: 100px 0;
}


/* =========================
   NAVBAR
========================= */

.navbar {
    position: absolute;
    top: 0;
    width: 100%;
    z-index: 100;
    padding: 25px 0;
}

.nav-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-size: 1.3rem;
    font-weight: 800;
    letter-spacing: 1px;
}

.logo span {
    color: #20d873;
}

nav {
    display: flex;
    gap: 30px;
}

nav a {
    font-size: 0.9rem;
    font-weight: 500;
    opacity: 0.85;
    transition: 0.3s;
}

nav a:hover {
    color: #20d873;
    opacity: 1;
}

.menu-toggle {
    display: none;
    border: none;
    background: none;
    color: white;
    font-size: 28px;
    cursor: pointer;
}


/* =========================
   HERO
========================= */

.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;

    background-image:
        url("https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=1800&q=85");

    background-size: cover;
    background-position: center;
    position: relative;
}

.hero-overlay {
    position: absolute;
    inset: 0;

    background:
        linear-gradient(
            90deg,
            rgba(5, 7, 9, 0.95),
            rgba(5, 7, 9, 0.65),
            rgba(5, 7, 9, 0.35)
        );
}

.hero-content {
    position: relative;
    z-index: 2;
    max-width: 720px;
    margin-left: max(5%, calc((100% - 1120px) / 2));
}

.eyebrow {
    color: #20d873;
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 2px;
    margin-bottom: 15px;
}

.hero h1 {
    font-size: clamp(3rem, 7vw, 6rem);
    line-height: 0.95;
    letter-spacing: -4px;
    margin-bottom: 25px;
}

.hero h1 span {
    color: #20d873;
}

.hero-text {
    max-width: 550px;
    font-size: 1.1rem;
    color: #d0d0d0;
    margin-bottom: 35px;
}

.hero-buttons {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
}

.btn {
    padding: 14px 24px;
    border-radius: 8px;
    font-weight: 700;
    transition: 0.3s;
}

.btn-primary {
    background: #20d873;
    color: #061009;
}

.btn-primary:hover {
    transform: translateY(-3px);
}

.btn-outline {
    border: 1px solid rgba(255,255,255,0.4);
    background: rgba(255,255,255,0.05);
}

.btn-outline:hover {
    background: white;
    color: #111;
}


/* =========================
   HEADINGS
========================= */

.section-heading {
    max-width: 650px;
    margin-bottom: 50px;
}

.section-heading h2,
.about-content h2,
.contact h2 {
    font-size: clamp(2rem, 5vw, 3.5rem);
    line-height: 1.1;
    letter-spacing: -1.5px;
    margin-bottom: 18px;
}

.section-heading p:last-child,
.about-content p,
.contact p {
    color: #9da2a7;
}


/* =========================
   SERVICES
========================= */

.services-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 18px;
}

.service-card {
    position: relative;
    padding: 35px 25px;
    background: #13161a;
    border: 1px solid #24282d;
    border-radius: 15px;
    transition: 0.3s;
}

.service-card:hover {
    transform: translateY(-7px);
    border-color: #20d873;
}

.service-icon {
    font-size: 2rem;
    margin-bottom: 20px;
}

.service-card h3 {
    margin-bottom: 10px;
}

.service-card p {
    color: #8f969d;
    font-size: 0.9rem;
    min-height: 85px;
}

.price {
    margin-top: 20px;
    font-size: 1.8rem;
    font-weight: 800;
    color: #20d873;
}

.featured {
    border-color: #20d873;
}

.popular {
    position: absolute;
    top: 15px;
    right: 15px;

    background: #20d873;
    color: #07100a;

    font-size: 0.65rem;
    font-weight: 800;

    padding: 5px 8px;
    border-radius: 5px;
}


/* =========================
   ABOUT
========================= */

.about {
    background: #101317;
}

.about-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 70px;
    align-items: center;
}

.about-image img {
    height: 550px;
    object-fit: cover;
    border-radius: 20px;
}

.about-content p {
    margin-bottom: 20px;
}

.stats {
    display: flex;
    gap: 35px;
    margin-top: 35px;
}

.stats div {
    display: flex;
    flex-direction: column;
}

.stats strong {
    color: #20d873;
    font-size: 1.8rem;
}

.stats span {
    color: #858b91;
    font-size: 0.8rem;
}


/* =========================
   GALLERY
========================= */

.gallery {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
}

.gallery img {
    height: 280px;
    object-fit: cover;
    border-radius: 12px;
    transition: 0.4s;
}

.gallery img:hover {
    transform: scale(1.03);
}


/* =========================
   INFO
========================= */

.info-section {
    background: #101317;
}

.info-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
}

.info-card {
    background: #171a1f;
    border: 1px solid #282c31;
    border-radius: 15px;
    padding: 35px;
}

.info-icon {
    font-size: 2rem;
    margin-bottom: 15px;
}

.info-card h3 {
    margin-bottom: 20px;
}

.info-card p {
    color: #999fa5;
    line-height: 1.9;
}

.hours div {
    display: flex;
    justify-content: space-between;
    padding: 12px 0;
    border-bottom: 1px solid #292d32;
}

.hours span {
    color: #969ba0;
}

.text-link {
    display: inline-block;
    margin-top: 20px;
    color: #20d873;
    font-weight: 700;
}


/* =========================
   CONTACT
========================= */

.contact-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 40px;
}

.contact-details {
    display: flex;
    flex-direction: column;
    gap: 18px;
}

.contact-details a {
    font-weight: 600;
    transition: 0.3s;
}

.contact-details a:hover {
    color: #20d873;
}


/* =========================
   FOOTER
========================= */

footer {
    padding: 35px 0;
    background: #070809;
    border-top: 1px solid #202328;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 30px;
}

.footer-content p {
    color: #777d83;
    font-size: 0.85rem;
}


/* =========================
   WHATSAPP
========================= */

.whatsapp {
    position: fixed;
    right: 25px;
    bottom: 25px;

    width: 60px;
    height: 60px;

    border-radius: 50%;

    background: #25D366;

    display: flex;
    justify-content: center;
    align-items: center;

    font-size: 1.6rem;

    box-shadow: 0 8px 30px rgba(0,0,0,0.4);

    z-index: 200;

    transition: 0.3s;
}

.whatsapp:hover {
    transform: scale(1.1);
}


/* =========================
   MOBILE
========================= */

@media (max-width: 900px) {

    .services-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .gallery {
        grid-template-columns: repeat(2, 1fr);
    }

    .about-grid {
        grid-template-columns: 1fr;
    }

    .about-image img {
        height: 400px;
    }

}


@media (max-width: 650px) {

    .section {
        padding: 70px 0;
    }

    .menu-toggle {
        display: block;
    }

    nav {
        position: absolute;
        top: 75px;
        right: 5%;

        width: 200px;

        background: #15181c;

        padding: 20px;

        border-radius: 10px;

        display: none;
        flex-direction: column;
        gap: 18px;

        border: 1px solid #292d32;
    }

    nav.active {
        display: flex;
    }

    .hero {
        min-height: 90vh;
    }

    .hero-content {
        margin-left: 5%;
    }

    .hero h1 {
        letter-spacing: -2px;
    }

    .services-grid,
    .gallery,
    .info-grid {
        grid-template-columns: 1fr;
    }

    .gallery img {
        height: 250px;
    }

    .contact-container {
        flex-direction: column;
        align-items: flex-start;
    }

    .footer-content {
        flex-direction: column;
        align-items: flex-start;
    }

    .stats {
        gap: 20px;
    }

}# aludeweb.github.i