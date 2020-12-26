<script>
    import Mosaic from "./UI/Mosaic.svelte";

    let imgs = [
        { src: "https://i.ibb.co/YtJ2y9G/1.jpg", alt: "" },
        { src: "http://ibb.co.com/images/hbU7FiNv3EQ63dc24d8d6ae39de.jpg", alt: "" },
        { src: "http://ibb.co.com/images/1HT9k84EvBAf601084360e55fe8.jpg", alt: "" },
        { src: "http://ibb.co.com/images/cZbY6Y5YOTQcb4b637a06d1c85f.jpg", alt: "" },
        { src: "https://i.ibb.co/tLN0VZ1/3.jpg", alt: "" },
        { src: "http://ibb.co.com/images/rxQfoytWo5g50b4f8b5c051730a.jpg", alt: "" },
        { src: "https://i.ibb.co/Bw7knSx/7.jpg", alt: "" },
        { src: "https://i.ibb.co/cF4wp42/8.jpg", alt: "" },
        { src: "https://i.ibb.co/KKzWvpk/9.jpg", alt: "" },
        { src: "https://i.ibb.co/ch71Vd9/10.jpg", alt: "" },
    ];
</script>

<style>
    div {
        width: 80%;
        margin: 125px auto 0;
    }
    @media (max-width: 768px) {
        div {
            width: 100%;
        }
    }
    @media (max-width: 426px) {
        div {
            margin-top: 85px;
        }
    }
</style>

<div>
    <Mosaic {imgs} />
</div>
