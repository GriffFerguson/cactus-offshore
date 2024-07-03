<script>
    export let href;
    export let x;
    export let count;
    
    export const width = 867;
    export const height = 1300;
    export const leg = width * .2;
    export const hypotenuse = Math.sqrt(Math.pow(leg,2) + Math.pow(height, 2));
</script>

<mask id="cutter{count}">
    <rect {x} y=0 {width} {height} fill="white" />
    <path d="M{parseInt(x) + width} 0 l-{leg} {hypotenuse} h{leg} z" fill="black" />
</mask>
<image {href} {x} y="0" mask="url(#cutter{count})" />