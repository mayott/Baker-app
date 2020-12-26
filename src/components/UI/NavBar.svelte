<script>
    import NavLink from "./NavLink.svelte";
    export let navElems = [];
</script>

<style>
    nav {
        display: flex;
        justify-content: space-around;
        width: 320px;
    }
    @media (max-width: 674px) {
        nav {
            width: 100%;

            justify-content: space-between;
            padding: 0 10px;
        }
    }
    @media (max-width: 321px) {
        nav {
            width: 100%;
            padding: 0 5px;
        }
    }
</style>

<nav>
    {#each navElems as elem}
        <NavLink {...elem} />
    {/each}
</nav>
