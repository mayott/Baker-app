<script>
    import Mosaic from "./UI/Mosaic.svelte";

    let imgs = [
        { src: "https://i.ibb.co/YtJ2y9G/1.jpg", alt: "" },
        { src: "https://i.ibb.co/phpwMNN/hb-U7-Fi-Nv3-EQ.jpg", alt: "" },
        { src: "https://i.ibb.co/XxQmx4b/1-HT9k84-Ev-BA.jpg", alt: "" },
        { src: "https://i.ibb.co/Lvn9Yy4/c-Zb-Y6-Y5-YOTQ.jpg", alt: "" },
        { src: "https://i.ibb.co/tLN0VZ1/3.jpg", alt: "" },
        { src: "https://i.ibb.co/VMNjqyQ/rx-Qfoyt-Wo5g.jpg", alt: "" },
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
