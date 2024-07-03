<script>
	import ImageMask from "../components/ImageMask.svelte";

</script>
<svelte:head>
    <title>Cactus Offshore</title>
</svelte:head>

<svg viewBox="0 0 2947.8 1300" xmlns="http://www.w3.org/2000/svg">
    <!-- width: 3468, height: 1300 -->
    <style>
        image {
            width: 867px;
            height: 1300px;
        }
    </style>

    <image href="/images/homepage_3.jpg" x="2080.8" y="0" />
    <ImageMask href="/images/homepage_4.jpg" x="1387.2" count="3" />
    <ImageMask href="/images/homepage_1.jpg" x="693.6" count="2" />
    <ImageMask href="/images/homepage_2.jpg" x="0" count="1" />
    <rect x="0" y="0" width="2947.8" height="1300" fill="rgba(15,15,15,0.65)" />
    <foreignObject width="1179.12" height="520" x="450" y="390" text-anchor="center">
        <p class="large">Management & Engineering for Subsea Projects</p>
        <p>Cactus Offshore specializes in the planning, management and execution of subsea installation and decommissioning projects.</p>
        <p>We have extensive experience in engineering, procurement, fabrication, installation, commissioning and decommissioning and have a track record of completed projects in the North Sea, Gulf of Mexico, Far East, West Africa and the Eastern Mediterranean.</p>
    </foreignObject>
</svg>

<style>
    svg {
        width: 100vw;
    }
    svg p.large {
        font-size: 4rem;
        font-weight: bold;
        margin: 0;
        padding: 0;
    }
    p {
        color: white;
        font-size: 1.3rem;
    }
</style>