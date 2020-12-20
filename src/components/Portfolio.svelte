<script>
    import Mosaic from "./UI/Mosaic.svelte";

    let imgs = [
        { src: "https://i.ibb.co/YtJ2y9G/1.jpg", alt: "" },
        { src: "https://i.ibb.co/VQWYRg1/2.jpg", alt: "" },
        { src: "https://i.ibb.co/tLN0VZ1/3.jpg", alt: "" },
        { src: "https://i.ibb.co/jbZDhJM/4.jpg", alt: "" },
        { src: "https://i.ibb.co/rQFjjr2/5.jpg", alt: "" },
        { src: "https://i.ibb.co/VLZtrNR/6.jpg", alt: "" },
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
