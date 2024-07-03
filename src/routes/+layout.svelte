<script>
    import Navlink from "../components/Navlink.svelte";
    import "../global.css";
</script>

<header>
    <img src="/horizontal.svg" alt="Cactus Offshore" role="heading" aria-level="1">
    <div id="nav-wrapper">
        <nav>
            <Navlink href="/">Home</Navlink>
            <Navlink href="/about">About</Navlink>
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
        position: relative;
        z-index: 999;
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
        width: 24%;
        display: inline-flex;
        flex-direction: row;
        justify-content: center;
        gap: 0.5rem;
        padding: 0.7vh 0;
    }

    #nav-wrapper::before, #nav-wrapper::after {
        content: "";
        width: 38%;
        height: 1px;
        background-color: rgb(35,35,35);
        display: inline-block;
    }

    footer {
        position: relative;
        bottom: 0.5vh;
        font-size: 0.84rem;
        font-family: "Raleway", sans-serif;
        color: rgb(35,35,35);
        width: 100%;
        text-align: center;
        padding: 1vh 0;
    }
    @media screen and (max-width: 1800px) {
        nav {
            width: 34%;
        }
        #nav-wrapper::before, #nav-wrapper::after {
            width: 33%;
        }
    }

    @media screen and (max-width: 1100px) {
        header {
            width: 65%;
            margin: 0 17.5%;
        }
    }

    @media screen and (max-width: 650px) {
        nav {
            width: 52%;
        }
        #nav-wrapper::before, #nav-wrapper::after {
            width: 24%;
        }
        header {
            width: 80%;
            margin: 0 10%;
        }
        header img {
            width: 70%;
            margin: 0 15%;
        }
    }
</style>