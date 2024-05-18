<template>
    <footer class="footer">
        <div class="container mx-auto">
            <div class="footer__content">
                <div class="lang-social">
                     <div class="language">
                         <img  class="language__image"src="../assets/images/icons/pt-BR.png" alt="bandeira do Brasil">
                         <span class="language__span text-sm">Português (Brasil)</span>
                         <img src="../assets/images/icons/arrow-icon.svg" alt="">
                     </div>
                     <div class="social">
                         <ul class="social__list">
                             <li class="social__list__item">
                                 <a href="#">
                                     <img src="../assets/images/social/x-icon.svg" alt="icone do X">
                                 </a>
                             </li>
                             <li class="social__list__item">
                                 <a href="#">
                                     <img src="../assets/images/social/instagram-icon.svg" alt="icone do instagram">
                                 </a>
                             </li>
                             <li class="social__list__item">
                                 <a href="#">
                                     <img src="../assets/images/social/facebook-icon.svg" alt="icone do facebook">
                                 </a>
                             </li>
                             <li class="social__list__item">
                                 <a href="#">
                                     <img src="../assets/images/social/youtube-icon.svg" alt="icone do youtube">
                                 </a>
                             </li>
                             <li class="social__list__item">
                                 <a href="#">
                                     <img src="../assets/images/social/tiktok-icon.svg" alt="icone do tiktok">
                                 </a>
                             </li>
                         </ul>
                     </div>
                 </div>
                 <nav class="footer__nav">
                     <ul class="footer__nav__list">
                         <li class="footer__nav__list__item">
                             <h3>Produto</h3>
                             <ul>
                                <li><a class="footer__item__link" href="#">Baixar</a></li>
                                <li><a class="footer__item__link" href="#">Nitro</a></li>
                                <li><a class="footer__item__link" href="#">Status</a></li>
                             </ul>
                         </li>
                         <li class="footer__nav__list__item">
                             <h3>Empresa</h3>
                             <ul>
                                <li><a class="footer__item__link" href="#">Sobre</a></li>
                                <li><a class="footer__item__link" href="#">Empregos</a></li>
                                <li><a class="footer__item__link" href="#">Marca</a></li>
                             </ul>
                         </li>
                         <li class="footer__nav__list__item">
                             <h3>Recursos</h3>
                             <ul>
                                <li><a class="footer__item__link" href="#">Faculdade</a></li>
                                <li><a class="footer__item__link" href="#">Suporte</a></li>
                                <li><a class="footer__item__link" href="#">Proteção</a></li>
                             </ul>
                         </li>
                         <li class="footer__nav__list__item">
                             <h3>Politica</h3>
                             <ul>
                                <li><a class="footer__item__link" href="#">Termos</a></li>
                                <li><a class="footer__item__link" href="#">Privacidade</a></li>
                                <li><a class="footer__item__link" href="#">Configurações de cookies</a></li>
                             </ul>
                         </li>
                     </ul>
                 </nav>
            </div>
            <hr>
            <div class="footer__content-2">
                <img class="footer__logo" src="../assets/images/devices/discord-logo.svg" alt="logo do discord">
                <button class="btn footer__btn">Registrar</button>
            </div>
        </div>
    </footer>
</template>

<style>
    .footer {
        @apply pb-16 pt-20;
        background: linear-gradient(#23272a 0%, #1e2124 47%, #141618 100%);
    }

    .footer__content {
        @apply flex items-center gap-[140px];
    }

    .language {
        @apply flex items-center gap-2 my-6 cursor-pointer;
    }

    .language__image {
        @apply  h-4 w-auto;
    }

    .language__span {
        font-family: ABCGin;
    }

    .social {
        margin-top: 24px
    } 
    
    .social__list {
        @apply flex items-center gap-6 
    }

    .social__list__item {
        @apply cursor-pointer h-[26px];
    }

    .footer__nav__list{
        @apply flex gap-6;
    }

    .footer__nav__list__item {
        width: 180px;
    }

    .footer__nav__list__item h3 {
        font-family: ABCGin;
        margin-bottom: 20px;
        color: rgba(88, 101, 242, 0.74);
    }

    .footer__nav__list__item ul {
        @apply flex flex-col gap-2;
    }

    .footer__item__link {
        font-family: ABCGin;
    }
    .footer__item__link:hover {
        text-decoration: underline;
    }
    
    hr {
        @apply my-8;
        background: rgb(88, 101, 242);
    }

    .footer__content-2 {
        @apply flex items-center justify-between
    }

    .footer__logo {
        width: 124px;
    }

    .footer__btn {
        background: rgb(88, 101, 242);
    }

    
</style>