<script>
    import About from "./About.svelte";
    import NavBar from "./UI/NavBar.svelte";

    let navElems = [
        { title: "О себе", href: "#about" },
        { title: "Написать мне", href: "#getintouch" },
    ];
</script>

<style>
    header {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        height: 64px;
        background: #323232 url(https://i.ibb.co/4Rp8TwS/Logo.png) no-repeat
            center;
        background-position: bottom;
    }
    header::after {
        position: absolute;
        content: "";
        background: #323232;
        width: 100px;
        height: 32px;
        left: calc(50% - 50px);
        top: 62px;
        clip-path: polygon(50% 100%, 0 0, 100% 0);
    }
</style>

<header>
    <NavBar {navElems} />
</header>
