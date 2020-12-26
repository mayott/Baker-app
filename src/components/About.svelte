<script>
    import App from "../App.svelte";
    import HexagonImg from "./UI/HexagonImg.svelte";
    let imgSrc = {
        src: "https://i.ibb.co/tD4KCtk/person.jpg",
        alt: "Пекарь Дима",
    };
    let size = "big";
</script>

<style>
    h1,
    p,
    ul {
        margin-bottom: 0;
        color: #d7fcf5;
    }
    li {
        line-height: 1.6;
    }
    h3 {
        color: #20816d;
    }
    h1,
    h3 {
        font-weight: 500;
        margin: 0;
    }
    a {
        text-decoration: none;
        color: inherit;
        cursor: default;
    }
    ul {
        margin: 0;
    }
    div.about {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 100px;
        background-color: #2eb398;
        height: 400px;
    }
    .text-group {
        margin-left: 25px;
        margin-top: -75px;
        position: relative;
    }
    .socials {
        position: absolute;
        bottom: -40px;
        right: 30px;

        width: 50px;
        height: 20px;
    }
    .socials a {
        font-size: 0;
        position: relative;
    }
    .vk::before {
        content: "";
        background-image: url("https://i.ibb.co/vVW1PPj/iconfinder-Logo-vk-Vkontakte-6214734.webp");
        background-size: cover;
        position: absolute;
        width: 40px;
        height: 40px;
        bottom: -20px;
        left: 0;
        cursor: pointer;
    }
    .inst::before {
        content: "";
        background-image: url("https://i.ibb.co/4skhQDy/iconfinder-Social-Media-Instagram-Outline-2959748.webp");
        background-size: cover;
        position: absolute;
        width: 40px;
        height: 40px;
        bottom: -20px;
        left: 40px;
        cursor: pointer;
    }
    @media (max-width: 1024px) {
        .about {
            padding: 0 30px;
        }
    }
    @media (max-width: 768px) {
        .text-group {
            margin-top: -25px;
        }
    }
    @media (max-width: 426px) {
        .vk::before,
        .inst::before {
            width: 45px;
            height: 45px;
        }
        div.about {
            flex-direction: column;
            height: 100%;
            margin-top: 50px;
            padding: 40px 30px 65px;
        }
        h1 {
            text-align: center;
            font-size: 24px;
        }
        h3 {
            text-align: center;
            font-size: 16px;
        }
        p,
        ul {
            font-size: 14px;
        }
        .text-group {
            margin: 0;
        }
        .socials {
            right: 50%;
        }
    }
</style>

<div class="about">
    <HexagonImg {...imgSrc} {size} />
    <div class="text-group">
        <h1><a name="about">Дмитрий Васьковский</a></h1>
        <h3>Слоёный перфекционист и пекарь.</h3>
        <p>Три кита на которых стоят мои убеждения об изделиях:</p>
        <ul>
            <li>
                нет лучше хлеба, чем хлеб на закваске;
            </li>
            <li>пористость и вкус расскажет о профессионализме твоего пекаря;</li>
            <li>только выдавая каждый день стабильный, качественный результат можно быть довольным своей работой.</li>
        </ul>
        <div class="socials">
            <a href="https://vk.com/" target="_blank" class="vk">VK</a>
            <a
                href="https://www.instagram.com/"
                target="_blank"
                class="inst">INSTAGRAM</a>
        </div>
    </div>
</div>
