<script>
    // No script needed for now
</script>

<header>
    <h1>Rickde Laundry Services</h1>
    <p>Professional. Reliable. On Time.</p>
</header>

<main>
    <slot />
</main>

<footer>
    &copy; {new Date().getFullYear()} Rickde Laundry Services. All rights reserved.
</footer>

<style>
    body {
        margin: 0;
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        background-color: #fff;
        color: #333;
    }

    header,
    footer {
        background-color: #4c6cc9;
        color: white;
        padding: 1rem;
        text-align: center;
    }

    footer {
        margin-top: 4rem;
    }

    main {
        padding: 0;
        margin: 0;
    }

    a {
        color: inherit;
        text-decoration: none;
    }

    a:hover {
        text-decoration: underline;
    }
</style>
