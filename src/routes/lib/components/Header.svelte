<script>
    function scrollToSection(id) {
        document.getElementById(id)?.scrollIntoView({ behavior: "smooth" });
    }
</script>

<header class="header">
    <div class="logo">
        <img src="/favicon.png" alt="Rickde Laundry Logo" />
        <span>Rickde Laundry</span>
    </div>

    <nav class="nav-links">
        <button on:click={() => scrollToSection("about")}>About</button>
        <button on:click={() => scrollToSection("services")}>Services</button>
        <button on:click={() => scrollToSection("testimonials")}
            >Testimonials</button
        >
        <button on:click={() => scrollToSection("contact")}>Contact</button>
    </nav>
</header>

<style>
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: white;
        padding: 1rem 2rem;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        position: sticky;
        top: 0;
        z-index: 100;
    }

    .logo {
        display: flex;
        align-items: center;
        gap: 0.5rem;
        font-weight: bold;
        font-size: 1.2rem;
    }

    .logo img {
        height: 32px;
        width: 32px;
        border-radius: 50%;
    }

    .nav-links button {
        background: none;
        border: none;
        font-size: 1rem;
        margin-left: 1rem;
        cursor: pointer;
        color: #333;
        font-weight: 500;
        transition: color 0.2s ease;
    }

    .nav-links button:hover {
        color: #25d366;
    }
</style>
