<script>
    export let title = "link name";
    export let href = "link href";
</script>

<style>
    a {
        font-weight: 500;
        font-size: 18px;
        text-decoration: none;
        color: rgb(224, 224, 224);
        padding: 5px;
    }
    a:hover {
        color: #37a78e;
    }
    @media (max-width: 426px) {
        a {
            font-size: 12px;
        }
    }
</style>

<a {href}>{title}</a>
