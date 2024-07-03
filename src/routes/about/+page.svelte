<script>
	import GalleryImage from "../../components/GalleryImage.svelte";

</script>
<svelte:head>
    <title>What We Do | Cactus Offshore</title>
</svelte:head>

<div id="content-wrapper">
    <img src="/images/helicopter.jpg" alt="helicopter landing" />
    <h2>About Us</h2>
    <p>Our personnel have provided onshore and offshore management and engineering services to operators and installation contractors on multiple projects.</p>
<p>Our expertise includes reeled rigid pipelines, large diameter S-lay trunklines, flexible flowlines and umbilicals, rigid and flexible jumpers, diverless connection systems, spool tie-ins, surface and saturation diving, production manifolds, PLETs and structures, spoolbase management, fabrication and operations.</p>
</div>

<div id="gallery">
    <GalleryImage src="/image_gallery/crane_ops.jpg" alt="crane lowering equipment into the ocean" />
    <GalleryImage src="/image_gallery/diving.jpg" alt="diving equipment" />
    <GalleryImage src="/image_gallery/equipment1.jpg" alt="pipe/umbilical equipment" />
    <GalleryImage src="/images/homepage_1.jpg" alt="robotic arm on a workbench" />
    <GalleryImage src="/image_gallery/fabrication1.jpg" alt="pipes in a fabrication shop" />
    <GalleryImage src="/image_gallery/diving2.jpg" alt="divers working on a pipeline underwater" />
    <GalleryImage src="/image_gallery/equipment2.jpg" alt="pipeline being held above a ship's deck with a crane" />
    <GalleryImage src="/images/homepage_3.jpg" alt="welder fabricating equipment" />
    <GalleryImage src="/image_gallery/platform1.jpg" alt="worker servicing equipment on an offshore platform" />
    <GalleryImage src="/image_gallery/diving3.jpg" alt="picture from the camera of an underwater vehicle" />
    <GalleryImage src="/images/homepage_2.jpg" alt="pipeline entering the ocean" />
    <GalleryImage src="/images/homepage_4.jpg" alt="person wearing protective clothing standing on a boat, with an oil platform in the background" />
</div>

<style>
    #content-wrapper {
        margin: 0 30%;
        width: 40%;
    }

    #gallery {
        margin: 0 30%;
        width: 40%;
        display:flex;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 0;
    }

    img {
        width: 100%;
        border-radius: 15px;
    }
</style>