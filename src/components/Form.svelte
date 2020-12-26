<script>
</script>

<style>
    div.form {
        background: #323232;
        padding: 85px 15px;
        color: #e0e0e0;
        display: flex;
        justify-content: center;
    }
    form {
        display: flex;
        flex-direction: column;
        width: 600px;
    }
    h2 {
        margin: 0;
    }
    a {
        color: inherit;
        text-decoration: none;
    }
    input,
    textarea {
        background-color: #454545;
        color: #bebebe;
        border: none;
        padding: 15px;
    }
    button {
        background-color: #2eb398;
        text-transform: uppercase;
        color: #d7fcf5;
        border: none;
        padding: 15px 30px;
        align-self: flex-end;
        margin-top: 10px;
        cursor: pointer;
    }
    span,
    p {
        font-size: 13px;
        line-height: 1.5;
    }
    button:hover {
        background-color: #39c5a9;
    }
    .text-group {
        width: 350px;
        margin-left: 30px;
        display: flex;
        flex-direction: column;
        padding-top: 60px;
    }
    .icon {
        position: relative;
        display: block;
        padding-left: 25px;
    }
    .icon:hover {
        color: #2d9c86;
    }
    .icon::before {
        content: "";
        position: absolute;
    }
    .location::before {
        height: 11px;
        width: 7px;
        left: 1px;
        bottom: 4px;
        background-image: url(https://i.ibb.co/LRHpsNT/location.png);
    }
    .phone::before {
        height: 11px;
        width: 11px;
        left: -1px;
        bottom: 4px;
        background-image: url(https://i.ibb.co/sgLDY6q/phone.png);
    }
    .mail::before {
        height: 8px;
        width: 13px;
        left: -2px;
        bottom: 4px;
        background-image: url(https://i.ibb.co/M73Cxvc/mail.png);
    }
    @media (max-width: 768px) {
        div.form {
            padding: 70px 30px;
        }
    }
    @media (max-width: 650px) {
        p {
            text-align: center;
        }
        .location::before {
            background-image: none;
        }
        .phone::before {
            background-image: none;
        }
        .mail::before {
            background-image: none;
        }
        .icon {
            padding-left: 0;
        }
        a {
            line-height: 2;
            font-size: 28px;
        }
        h2 {
            text-align: center;
        }
        div.form {
            padding: 30px 20px;
            flex-direction: column;
        }
        form {
            width: 100%;
        }
        .text-group {
            width: 100%;
            padding-top: 10px;
            margin: 0 auto;
            text-align: center;
        }
        button {
            align-self: auto;
        }
    }
    @media (max-width: 350px) {
        a {
            line-height: 2;
            font-size: 18px;
        }
        form {
            font-size: 12px;
        }
    }
</style>

<div class="form">
    <form action="https://formspree.io/f/xvovqrab" method="POST" name="mess">
        <h2><a name="getintouch">Связаться со мной</a></h2>
        <p>Чтобы связаться со мной, используйте форму ниже:</p>
        <input type="text" placeholder="Ваше имя" name="name" />
        <input
            type="email"
            placeholder="Email для обратной связи"
            name="_replyto" />

        <input type="text" placeholder="Тема" name="_subject" />
        <input type="hidden" name="_next" value="//site.io/thanks.html" />
        <textarea cols="30" rows="10" placeholder="Сообщение" name="message" />
        <button>Отправить</button>
    </form>

    <div class="text-group">
        <p>
            Открыт для конструктивного диалога или обычной беседы. Постараюсь
            ответить в ближайшее свободное время. Если данный канал коммункации
            не подходит, ниже оставлю свою почту и рабочий номер телефона.
        </p>

        <span class="icon phone"><a href="tel:+79998887766">+7 (999) 888-77-66</a></span>
        <span class="icon mail"><a
                href="mailto:mail@gmail.com">mail@gmail.com</a></span>
        <span class="icon location"><a
                href="https://goo.gl/maps/fiPEuL77HaoQSNrC9"
                target="_blank">Москва, г. Московский</a></span>
    </div>
</div>
