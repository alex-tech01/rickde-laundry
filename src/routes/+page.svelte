<script>
    // JS logic if needed
</script>

<!-- Header -->
<header class="header">
    <div class="branding">
        <h1>Rickde Laundry</h1>
        <p class="tagline">“Because your clothes deserve the best care.”</p>
    </div>
</header>

<!-- Hero Section -->
<section class="hero">
    <div class="hero-content">
        <h1>Welcome to Rickde Laundry Services</h1>
        <p>Fresh. Fast. Flawless Laundry Services at Your Doorstep</p>

        <div class="nav-buttons">
            <button
                on:click={() =>
                    document
                        .getElementById("about")
                        .scrollIntoView({ behavior: "smooth" })}>About</button
            >
            <button
                on:click={() =>
                    document
                        .getElementById("services")
                        .scrollIntoView({ behavior: "smooth" })}
                >Services</button
            >
            <button
                on:click={() =>
                    document
                        .getElementById("testimonials")
                        .scrollIntoView({ behavior: "smooth" })}
                >Testimonials</button
            >
            <button
                on:click={() =>
                    document
                        .getElementById("contact")
                        .scrollIntoView({ behavior: "smooth" })}>Contact</button
            >
        </div>
    </div>
</section>

<!-- About Section -->
<section class="section" id="about">
    <h2>About Us</h2>
    <p>
        Welcome to Rickde Laundry! We provide professional, affordable, and
        on-time laundry services. With a passion for clean clothes and happy
        clients, we’re here to take the stress out of your laundry day.
    </p>
</section>

<!-- Services Section -->
<section class="section" id="services">
    <h2>Our Services</h2>
    <ul>
        <li>🧺 Pick-Up & Delivery</li>
        <li>👚 Dry Cleaning</li>
        <li>🧼 Wash & Fold</li>
        <li>🧻 Ironing & Steaming</li>
        <li>🚀 Same Day Service</li>
        <li>🌿 Eco-Friendly Options</li>
    </ul>
</section>

<!-- Testimonials Section -->
<section class="section" id="testimonials">
    <h2>What Our Clients Say</h2>
    <div class="testimonials">
        <div class="testimonial">
            "Reliable and fast! Rickde Laundry is a life-saver for my busy
            schedule." – Janet K.
        </div>
        <div class="testimonial">
            "My clothes come back cleaner than ever. Highly recommend!" – Peter
            M.
        </div>
        <div class="testimonial">
            "They even folded my socks perfectly! Love the service." – Linda O.
        </div>
    </div>
</section>

<!-- Contact Section -->
<section class="section" id="contact">
    <h2>Get in Touch</h2>
    <p>Want to schedule a pickup or ask us something? Chat with us now 👇</p>
    <a
        href="https://wa.me/254741803693"
        target="_blank"
        rel="noopener"
        class="whatsapp-button"
    >
        📲 Chat on WhatsApp
    </a>
</section>

<!-- Footer -->
<footer>
    <p>
        &copy; {new Date().getFullYear()} Rickde Laundry Services. All rights reserved.
    </p>
</footer>

<!-- Floating WhatsApp Icon -->
<a
    href="https://wa.me/254741803693"
    class="floating-whatsapp"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Chat with us on WhatsApp"
>
    🟢
</a>

<style>
    /* Header */
    .header {
        background: linear-gradient(to right, #667eea, #764ba2);
        color: white;
        padding: 2rem 1rem;
        text-align: center;
        box-shadow: 0 2px 10px rgba(0, 0, 0, 0.15);
    }
    .branding h1 {
        font-size: 2.5rem;
        margin: 0;
        font-weight: 700;
    }
    .tagline {
        font-size: 1.2rem;
        margin-top: 0.5rem;
        font-style: italic;
        opacity: 0.9;
    }

    /* Hero */
    .hero {
        background: url("/laundry-hero.jpg") center/cover no-repeat;
        height: 40vh;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        text-align: center;
        padding: 2rem;
        text-shadow: 1px 1px 5px #000;
    }
    .hero-content {
        background-color: rgba(0, 0, 0, 0.4);
        padding: 2rem;
        border-radius: 10px;
    }
    .hero h1 {
        font-size: 3rem;
        margin-bottom: 0.5rem;
    }
    .hero p {
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
    }
    .nav-buttons {
        display: flex;
        gap: 1rem;
        flex-wrap: wrap;
        justify-content: center;
    }
    .nav-buttons button {
        padding: 0.7rem 1.5rem;
        border: 2px solid white;
        background: transparent;
        color: white;
        border-radius: 25px;
        cursor: pointer;
        font-weight: bold;
        transition: all 0.3s ease;
    }
    .nav-buttons button:hover {
        background: white;
        color: black;
    }

    /* Sections */
    .section {
        max-width: 960px;
        margin: 3rem auto;
        padding: 0 1rem;
        text-align: center;
    }
    .section h2 {
        font-size: 2rem;
        margin-bottom: 1rem;
    }
    .section ul {
        list-style: none;
        padding: 0;
    }
    .section li {
        margin-bottom: 0.5rem;
        font-size: 1.1rem;
    }

    /* Testimonials */
    .testimonials {
        display: grid;
        gap: 1rem;
        margin-top: 1rem;
    }
    .testimonial {
        background: #f3f3f3;
        padding: 1rem;
        border-radius: 8px;
    }

    /* Contact Button */
    .whatsapp-button {
        display: inline-block;
        margin-top: 1rem;
        padding: 0.7rem 1.5rem;
        background: #25d366;
        color: white;
        border-radius: 5px;
        text-decoration: none;
        font-weight: bold;
    }

    /* Footer */
    footer {
        text-align: center;
        padding: 2rem 1rem;
        background: #222;
        color: white;
    }

    /* Floating WhatsApp Icon */
    .floating-whatsapp {
        position: fixed;
        bottom: 20px;
        right: 20px;
        background-color: #25d366;
        color: white;
        font-size: 2rem;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        text-decoration: none;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
        transition: transform 0.3s ease;
        z-index: 1000;
    }
    .floating-whatsapp:hover {
        transform: scale(1.1);
    }
</style>
