<script>
    import Navlink from "../components/Navlink.svelte";
    import "../global.css";
</script>

<header>
    <img src="/logo.png" alt="Cactus Offshore" role="heading" aria-level="1">
    <div id="nav-wrapper">
        <nav>
            <Navlink href="/">Home</Navlink>
            <Navlink href="/about">About</Navlink>
            <Navlink href="/services">Services</Navlink>
        </nav>
    </div>
</header>

<main>
    <slot></slot>
</main>

<footer>
    Cactus Offshore &copy; 2024
</footer>

<style>
    header {
        width: 35%;
        margin: 0 32.5%;
        padding: 3vh 0;
    }

    header > img {
        width: 50%;
        margin: 0 25%;
    }

    #nav-wrapper {
        width: 100%;
    }

    nav {
        width: 32%;
        display: inline-flex;
        flex-direction: row;
        justify-content: center;
        gap: 0.5rem;
        padding: 0.7vh 0;
    }

    #nav-wrapper::before, #nav-wrapper::after {
        content: "";
        width: 34%;
        height: 1px;
        background-color: rgb(35,35,35);
        display: inline-block;
    }

    footer {
        position: absolute;
        bottom: 0.5vh;
        font-size: 0.84rem;
        font-family: "Raleway", sans-serif;
        color: rgb(35,35,35);
        width: 100%;
        text-align: center;
        padding: 0.5vh 0;
    }
</style>