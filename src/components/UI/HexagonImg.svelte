<script>
    export let src = "/";
    export let alt = "Картинка";
    export let size = "normal";
</script>

<style>
    img {
        clip-path: polygon(50% 0, 100% 25%, 100% 75%, 50% 100%, 0 75%, 0 25%);
        width: 180px;
        height: 200px;
        margin: 5px;
        margin-top: -45px;
    }
    @media (max-width: 768px) {
        img {
            width: 150px;
            height: 165px;
            margin-top: -35px;
        }
    }
    @media (max-width: 426px) {
        img {
            width: 80px;
            height: 93px;
            margin-top: -25px;
        }
        img.big {
            width: 150px;
            height: 165px;
        }
    }
</style>

<img {src} {alt} class={size === 'big' ? 'big' : ''} />
