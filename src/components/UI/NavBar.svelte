<script>
    import NavLink from "./NavLink.svelte";
    export let navElems = [];
</script>

<style>
    nav {
        display: flex;
        justify-content: space-around;
        width: 450px;
    }
    @media (max-width: 768px) {
        nav {
            width: 320px;
        }
    }
    @media (max-width: 426px) {
        nav {
            width: 100%;

            justify-content: space-between;
            padding: 0 30px;
        }
    }
</style>

<nav>
    {#each navElems as elem}
        <NavLink {...elem} />
    {/each}
</nav>
