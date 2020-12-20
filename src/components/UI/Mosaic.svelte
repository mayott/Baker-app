<script>
    import HexagonImg from "./HexagonImg.svelte";
    export let imgs = [];

    function imgsLength(arr) {
        return console.log(arr.length);
    }
</script>

<style>
    div.mosaic {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        width: 760px;
        margin: 0 auto;
    }
    div.filler {
        width: 1px;
        height: 110px;
        background-color: #ccc;
    }
    @media (max-width: 768px) {
        div.mosaic {
            width: 640px;
        }
    }
    @media (max-width: 426px) {
        div.mosaic {
            width: 360px;
        }
        div.filler {
            height: 60px;
        }
    }
</style>

<div class="mosaic">
    <div class="filler" />
    {#each imgs as { src, alt }}
        <HexagonImg {src} {alt} />
    {/each}
    <div class="filler" />
</div>
