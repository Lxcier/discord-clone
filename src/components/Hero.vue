<template>
    <main class="hero">
        <div class="container mx-auto">
            <section class="hero__content">
                <div class="cta">
                    <h1 class="hero__title">
                        Baixe o Discord para qualquer dispositivo
                    </h1>
                    <p class="hero__paragraph">
                        Uma aventura aguarda. Reúna seus amigos no nosso app para área de trabalho e continue o papo em qualquer lugar pelo celular.
                    </p>
                    <div class="buttons">
                        <a class="btn-2 cta__btn-download" href="#">
                            Baixar para Windows
                        </a>
                        <span class="cta__span">Windows 10 ou superior</span>
                    </div>
                </div>
                <div class="hero__image">
                    <img src="../assets/images/devices/discord-window.svg" alt="Disponivel no windows">
                </div>
            </section>
        </div>
    </main>
</template>

<style>
    .hero {
        @apply flex items-center justify-between flex-col pt-52 pb-32;
        background: linear-gradient(#23272a 0%, #1e2124 47%, #141618 100%);
        margin-top: -80px;
    }

    .hero__content {
        @apply flex items-center justify-between flex-row h-auto mx-auto gap-10;
    }

    .cta {
        @apply flex items-start justify-center flex-col relative gap-5;
    }

    .hero__title {
        @apply mb-6 font-bold uppercase;
        font-family: ABCGinNord;
        font-size: 50px;
        font-weight: 800;
        line-height: 50px;
        transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
        transform-style: preserve-3d;
    }

    .hero__paragraph {
        margin-bottom: 10px;
        font-family: GGSans, sans-serif;
        font-size: 20px;
        text-align: left;
    }

    .btn-2.cta__btn-download {
        background: #5865f2;
        background-image:url(https://assets-global.website-files.com/6257adef93867e50d84d30e2/6582b262413a0600bad70006_download.svg);
        background-position: 32px;
        background-repeat: no-repeat;
        background-size: auto;
        flex: none;
        padding-left: 66px;
    }

    .buttons {
        @apply flex items-center gap-5;
        flex-wrap: wrap;
    }

    .hero__image {
        @apply w-full relative
    }

    .hero__image img {
        width: 100%;
    }

    .cta__span {
        font-family: ABCGin;
    }
</style>