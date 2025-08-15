<script>
	import ImageMask from "../components/ImageMask.svelte";
    import GalleryImage from "../components/GalleryImage.svelte";
</script>
<svelte:head>
    <title>Cactus Offshore</title>
</svelte:head>

<div id="homepage">
    <svg viewBox="0 0 2947.8 1300" xmlns="http://www.w3.org/2000/svg">
        <!-- width: 3468, height: 1300 -->
        <style>
            image {
                width: 867px;
                height: 1300px;
            }
        </style>
    
        <g id="images">
            <image href="/images/homepage_3.jpg" x="2080.8" y="0" />
            <ImageMask href="/images/homepage_4.jpg" x="1387.2" count="3" />
            <ImageMask href="/images/homepage_1.jpg" x="693.6" count="2" />
            <ImageMask href="/images/homepage_2.jpg" x="0" count="1" />
        </g>
        <rect x="0" y="0" width="2947.8" height="1300" fill="rgba(15,15,15,0.65)" />
    </svg>
    <div id="title-card">
        <p class="large">Management & Engineering for Subsea Projects</p>
        <p>Cactus Offshore specializes in the planning, management and execution of subsea installation and decommissioning projects.</p>
        <p>We have extensive experience in engineering, procurement, fabrication, installation, commissioning and decommissioning and have a track record of completed projects in the North Sea, Gulf of Mexico, Far East, West Africa and the Eastern Mediterranean.</p>
    </div>
</div>

<hr/>

<div id="content-wrapper">
    <img src="/images/rov.jpg" alt="picture from the camera of an underwater vehicle" />
    <h2>About Us</h2>
    <p>Our personnel have provided onshore and offshore management and engineering services to operators and installation contractors on multiple projects.</p>
<p>Our expertise includes reeled rigid pipelines, large diameter S-lay trunklines, flexible flowlines and umbilicals, rigid and flexible jumpers, diverless connection systems, spool tie-ins, surface and saturation diving, production manifolds, PLETs and structures, spoolbase management, fabrication and operations.</p>
</div>

<div id="gallery">
    <GalleryImage src="/image_gallery/platform1.jpg" alt="worker servicing equipment on an offshore platform" />
    <GalleryImage src="/image_gallery/equipment2.jpg" alt="pipeline being held above a ship's deck with a crane" />
    <GalleryImage src="/image_gallery/fabrication1.jpg" alt="pipes in a fabrication shop" />
    <GalleryImage src="/image_gallery/diving2.jpg" alt="divers working on a pipeline underwater" />
    <GalleryImage src="/image_gallery/crane_ops.jpg" alt="crane lowering equipment into the ocean" />
    <GalleryImage src="/image_gallery/diving.jpg" alt="diving equipment" />
    <GalleryImage src="/image_gallery/equipment1.jpg" alt="pipe/umbilical equipment" />
    <GalleryImage src="/image_gallery/fabrication2.jpg" alt="welder inspecting a pipe" />
</div>

<style>
    /* IMAGE COLLAGE HEADER */
    #homepage {
        position: relative;
        width: 100%;
        height: 90vh;
    }

    svg {
        min-width: 100vw;
        min-height: 100%;
        position: absolute;
        top: 0;
        left: 0;
    }
    #homepage .large {
        font-size: 3.5rem;
        font-weight: bold;
        margin: 0;
        padding: 0;
        text-align: center;
    }
    #homepage p {
        color: white;
        font-size: 1rem;
        text-shadow: 1px 1px black, -1px -1px black;
    }

    #homepage p:not(.large) {
        width: 80%;
        margin: 1.4ch 10%;
    }

    #title-card {
        top: 30%;
        position: absolute;
        width: 50%;
        margin: 0 25%;
    }
    @media only screen and (max-width: 750px) {
        #homepage .large {
            font-size: 2.9rem;
        }

        #title-card {
            width: 80%;
            margin: 0 10%;
        }

        /* #images {
            animation-name: imageSlideshow;
            animation-duration: 16s;
            animation-timing-function: ease-out;
            animation-iteration-count: infinite;
        }

        @keyframes imageSlideshow {
            0%, 24% {
                x: 0px;
            }

            25%, 49% {
                x: 867px;
            }
            
            50%, 74% {
                x: 1734px;
            }
            
            75%, 99% {
                x: 2610px;
            }
        } */
    }
    @media only screen and (max-width: 500px) {
        #title-card {
            width: 94%;
            margin: 0 3%;
        }
    }

    /* ABOUT SECTION */

    #content-wrapper, #gallery{
        margin: 0 30%;
        width: 40%;
    }

    #gallery {
        display:flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 0;
    }

    img {
        width: 100%;
        border-radius: 15px;
    }

    @media screen and (max-width: 1400px) {
        #content-wrapper, #gallery {
            margin: 0 20%;
            width: 60%;
        }
    }
    
    @media screen and (max-width: 700px) {
        #content-wrapper, #gallery {
            margin: 0 10%;
            width: 80%;
        }
    }

    hr {
        margin: 5vh 10%;
        width: 80%;
        height: 0.01rem;
        background-color: black;
    }
</style>