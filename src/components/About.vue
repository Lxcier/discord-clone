<template>
    <section class="about">
        <div class="container mx-auto">
            <ul class="about__content">
                <li class="about__content__item ios">
                    <h2 class="about__content__item__title">iOS</h2>
                    <a href="#" class="btn about__content__item__link">Baixar</a>
                    <img class="about__content__item__image" src="../assets/images/devices/discord-ios.svg" alt="Disponivel no iOS">
                </li>
                <li class="about__content__item android">
                    <h2 class="about__content__item__title">Android</h2>
                    <a href="#" class="btn about__content__item__link">Baixar</a>
                    <img class="about__content__item__image" src="../assets/images/devices/discord-android.svg" alt="Disponivel no android">
                </li>
                <li class="about__content__item linux">
                    <h2 class="about__content__item__title">Linux</h2>
                    <a href="#" class="btn about__content__item__link">Baixar</a>
                    <img class="about__content__item__image" src="../assets/images/devices/discord-linux.svg" alt="Disponivel no linux">
                </li>
                <li class="about__content__item mac">
                    <h2 class="about__content__item__title">Mac</h2>
                    <a href="#" class="btn about__content__item__link">Baixar</a>
                    <img class="about__content__item__image" src="../assets/images/devices/discord-mac.svg" alt="Disponivel no mac">
                </li>
                <li class="about__content__item beta">
                    <h2 class="about__content__item__title">Gosta de viver perigosamente?</h2>
                    <p class="about__content__item__paragraph">Experimente nossa Versão de Teste Público e confira recursos novos antes deles saírem.</p>
                    <div class="dropdown">
                        <button class="dropdown__btn btn" type="button">
                            <span class="dropdown__btn__span">Baixar a versão pública de teste</span>
                            <img src="../assets/images/icons/arrow-icon.svg" alt="">
                        </button>
                        <nav class="dropdown-menu">
                            <ul class="dropdown-menu__list">
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Mac</a>
                                </li>
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Linux deb</a>
                                </li>
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Linux tar.gz</a>
                                </li>
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Windows 64-bit</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                </li>

                <li class="about__content__item older">
                    <h2 class="about__content__item__title">Dos arquivos:</h2>
                    <p class="about__content__item__paragraph">Usuários do Windows 7/8/8.1 e do Windows 32-bit podem baixar o aplicativo oficial, porém sem suporte, aqui.</p>
                    <div class="dropdown">
                        <button class="dropdown__btn btn" type="button">
                            <span class="dropdown__btn__span">Baixar</span>
                            <img src="../assets/images/icons/arrow-icon.svg" alt="">
                        </button>
                        <nav class="dropdown-menu">
                            <ul class="dropdown-menu__list">
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Windows 7/8/8.1 (disponível até 15 de junho de 2024)</a>
                                </li>
                                <li class="dropdown-menu__list__item">
                                    <a class="dropdown-menu__list__item__link" href="#">Windows 32-bit (disponível até 15 de junho de 2024)</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                </li>
            </ul>
        </div>
    </section>
</template>

<style>
    .about {
        @apply pt-32 pb-16;
        background: #e9e9e9;
    }

    .about p, .about h2{
        color: rgb(6, 10, 11);
    }

    .about__content {
        @apply grid grid-cols-2 auto-cols-fr gap-5;
        grid-template-rows: minmax(auto, 160px) minmax(auto, 420px) minmax(auto, 160px) auto minmax(auto, 120px) auto;
    }

    .about__content__item {
        @apply flex flex-col items-center rounded-2xl max-h-[600px] h-full overflow-x-hidden overflow-y-hidden p-14;
        background:  rgb(246, 246, 246);
    }

    .about__content__item.ios {
        grid-area: 1 / 1 / 3 / 2;
        text-size-adjust: 100%;
    }

    .android {
        grid-area: 2 / 2 / 4 / 3;
    }

    .linux {
        grid-area: span 2 / span 1 / span 2 / span 1;
    }

    .mac {
        grid-area: span 2 / span 1 / span 2 / span 1;
    }

    .beta, 
    .older {
        @apply relative py-12 px-10 h-full justify-start items-start gap-6 overflow-visible max-h-[324px];
    }

    .beta {
        grid-area: span 2 / span 1 / span 2 / span 1;
    }

    .about__content__item__title {
        @apply font-semibold text-4xl mb-2 text-center;
        font-family: ABCGin;
        line-height: 38px;
        margin-block-end: 8px;
        margin-block-start: 0;
        text-size-adjust: 100%;
    }

    .beta .about__content__item__title {
        @apply text-[32px];
    }

    .about__content__item__link{
        @apply flex items-center justify-center cursor-pointer text-xl mx-auto mt-3 max-h-14 max-w-full px-8 py-4 text-nowrap;
        text-size-adjust: 100%;
        white-space-collapse: collapse;
    }

    .about__content__item__image {
        @apply overflow-clip max-w-full mt-16;
        overflow-clip-margin: content-box;
    }

    .dropdown {
        @apply flex flex-col items-start relative text-left w-[500px] z-10
    }

    .dropdown__btn {
        @apply flex items-center gap-3 text-xl font-medium;
        padding: 12px 32px 15px;
    }

    .dropdown__btn__span,
    .about__content__item__paragraph
     {
        font-family: ABCGin, sans-serif;
    }

    .about__content__item__paragraph {
        @apply text-xl
    }

    .dropdown-menu {
        @apply absolute z-[11] p-4 mt-[60px] bg-white top-[0%] left-[0%] bottom-auto right-[0%] shadow-sm rounded-lg;
    }

    .dropdown-menu__list__item {
        @apply p-2 rounded transition-all text-[#222] w-full;
    }

</style>