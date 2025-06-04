<script>
    // No logic needed right now
</script>

<!-- Hero Section -->
<section class="hero">
    <h2>Welcome to Rickde Laundry Services</h2>
    <p>Your trusted partner for fresh, clean laundry — on time.</p>

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
                    .scrollIntoView({ behavior: "smooth" })}>Services</button
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
</section>

<!-- About Section -->
<section class="section" id="about">
    <h3>About Me</h3>
    <p>
        Hi! I'm Rickde, a passionate laundry service provider focused on making
        laundry effortless for you. I offer personalized care, fast turnaround,
        and unmatched convenience to busy homes and professionals.
    </p>
</section>

<!-- Services Section -->
<section class="section" id="services">
    <h3>Services Offered</h3>
    <div class="services">
        <div class="service-item">🧺 Pick-Up & Delivery</div>
        <div class="service-item">👚 Dry Cleaning</div>
        <div class="service-item">🧼 Wash & Fold</div>
        <div class="service-item">🧻 Ironing & Steaming</div>
        <div class="service-item">🚀 Same Day Service</div>
        <div class="service-item">🌿 Eco-Friendly Options</div>
    </div>
</section>

<!-- Testimonials Section -->
<section class="section" id="testimonials">
    <h3>What Our Clients Say</h3>
    <div class="services">
        <div class="service-item">
            “Reliable and fast! Rickde Laundry is a life-saver for my busy
            schedule.” – Janet K.
        </div>
        <div class="service-item">
            “My clothes come back cleaner than ever. Highly recommend!” – Peter
            M.
        </div>
        <div class="service-item">
            “They even folded my socks perfectly! Love the service.” – Linda O.
        </div>
    </div>
</section>

<!-- Contact Section -->
<section class="section" id="contact">
    <h3>Get in Touch</h3>
    <p>
        Have questions or want to schedule a pick-up? Reach out to us directly
        on WhatsApp!
    </p>

    <a
        href="https://wa.me/254741803693"
        target="_blank"
        rel="noopener"
        class="whatsapp-button"
    >
        📲 Chat on WhatsApp
    </a>
</section>

<style>
    .hero {
        background: url("/laundry-hero.jpg") center/cover no-repeat;
        height: 75vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: white;
        text-align: center;
        padding: 2rem;
        text-shadow: 1px 1px 5px #000;
    }

    .hero h2 {
        font-size: 2.5rem;
        margin-bottom: 0.5rem;
    }

    .hero p {
        font-size: 1.2rem;
        margin-bottom: 1rem;
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

    .section {
        max-width: 960px;
        margin: 3rem auto;
        padding: 0 1rem;
        text-align: center;
    }

    .section h3 {
        font-size: 2rem;
        margin-bottom: 1rem;
    }

    .services {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 1rem;
        margin-top: 2rem;
    }

    .service-item {
        background: #f3f3f3;
        padding: 1rem;
        border-radius: 8px;
        text-align: center;
        font-size: 0.95rem;
    }

    .whatsapp-button {
        display: inline-block;
        margin-top: 1rem;
        padding: 0.7rem 1.5rem;
        background: #25d366;
        color: white;
        border-radius: 5px;
        text-decoration: none;
        font-weight: bold;
        max-width: 280px;
        width: 100%;
    }

    /* 📱 Responsive Styling */
    @media (max-width: 600px) {
        .hero h2 {
            font-size: 1.8rem;
        }

        .hero p {
            font-size: 1rem;
        }

        .nav-buttons {
            flex-direction: column;
            align-items: center;
        }

        .nav-buttons button {
            width: 100%;
            max-width: 250px;
        }
    }
</style>
