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
        opacity: 0;
    }
    @media (max-width: 950px) {
        div.mosaic {
            width: 620px;
        }
    }
    @media (max-width: 650px) {
        div.mosaic {
            width: 360px;
        }
        div.filler {
            height: 60px;
        }
    }
    @media (max-width: 374px) {
        div.mosaic {
            width: 256px;
        }
        div.filler {
            height: 40px;
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
