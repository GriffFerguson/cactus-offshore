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
    <rect x="0" y="0" width="2947.8" height="1300" fill="rgba(30,30,30,0.5)" />
        <foreignObject width="1179.12" height="260" x="884.34" y="520" text-anchor="center">
            <p>Management & Engineering for Subsea Projects</p>
        </foreignObject>
</svg>



<style>
    svg {
        width: 100vw;
    }
    p{
        font-size: 5rem;
        color: white;
        font-weight: bold;
        text-align: center;
        margin: 0;
        padding: 0;
    }
</style>