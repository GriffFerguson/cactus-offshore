<script>
    export let src;
    export let alt;
    export let displayImage = false;

    function showImage() {
        displayImage = true;
    }

    function hideImage(e) {
        if (e.target.id == "image-viewer" || e.target.id == "image-viewer-container" || e.target.id == "image-viewer-close") {
            displayImage = false;
        }
    }
</script>

<div class="thumbnail" style:background-image="url({src})" on:click={showImage} role="button" tabindex="-1" />

{#if displayImage}
<div id="image-viewer" on:click={hideImage}>
    <div id="image-viewer-container">
        <img {src} {alt} />
        <button type="button" aria-label="Close" id="image-viewer-close">X</button>
    </div>
</div>
{/if}

<style>
    .thumbnail {
        width: 49%;
        margin: 0.5%;
        aspect-ratio: 16/10;
        display: block;
        background-size: cover;
        background-position: center center;
        cursor: pointer;
        background-repeat: no-repeat;
    }
    
    #image-viewer {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(10,10,10,0.7);
    }

    #image-viewer-container {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: flex;
        align-items: center;
        justify-content: center;
        max-width: 50%;
        max-height: 80%;
    }

    #image-viewer img {
        min-width: 25vw;
        width: auto;
        height: auto;
        border: 5px solid white;
        max-height: 80vh;
    }

    button {
        position: absolute;
        top:0;
        right: 0;
        transform: translate(50%, -50%);
        border-radius: 50%;
        width: 2rem;
        height: 2rem;
        border: 2px solid white;
        background-color: black;
        color: white;
        font-weight: bold;
        font-size: 1.2rem;
        text-align: center;
        cursor: pointer;
        padding: 0.3rem;
        margin: 0;
        line-height: 1.2rem;
        vertical-align: middle;
    }
    button:hover {
        background-color: rgb(50,50,50);
    }

    @media screen and (max-width: 900px) {
        #image-viewer-container {
            max-width: 90%;
            max-height: 85%;
        }
    }
</style>