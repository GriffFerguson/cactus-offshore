<script>
    import "../global.css";
</script>

<header>
    <img src="/logo.png" alt="Cactus Offshore" role="heading" aria-level="1">
    <div id="nav-wrapper">
        <nav>
            <a href="/">Home</a>
            <a href="/about">About</a>
            <a href="/services">Services</a>    
        </nav>
    </div>
</header>

<slot></slot>

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

    nav a {
        text-decoration: none;
        padding: 0.5rem 0.8rem;
        transition: background-color 0.4s;
    }

    nav a:hover {
        background-color: rgb(223, 223, 223);
        border-radius: 5%;
    }
    
    #nav-wrapper::before, #nav-wrapper::after {
        content: "";
        width: 34%;
        height: 1px;
        background-color: rgb(35,35,35);
        display: inline-block;
    }
</style>