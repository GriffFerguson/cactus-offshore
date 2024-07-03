<script>
    import { page } from "$app/stores";

    export let href;
    $: active = $page.url.pathname === href;
</script>

<a {href} class:active={active}>
    <slot></slot>
</a>

<style>
    a {
        text-decoration: none;
        padding: 0.5rem 0.8rem;
        transition: background-color 0.4s;
        font-size: 0.9rem;
    }

    a:hover {
        background-color: rgb(223, 223, 223);
        border-radius: 5%;
    }

    .active {
        background-color: rgb(236, 236, 236);
    }
</style>