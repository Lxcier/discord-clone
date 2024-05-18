<template>
    <header class="header container mx-auto">
        <a class="header__logo" href="https://discord.com/download">
            <img src="../assets/images/devices/discord-logo.svg" alt="Discord Logo">
        </a>
        <nav class="navbar">
            <ul class="navbar__list">
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Baixar</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Nitro</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Descobrir</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Proteção</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Suporte</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Blog</a></li>
                <li class="navbar__list__item"><a href="#" class="navbar__list__item__link">Carreiras</a></li>
            </ul>
        </nav>
        <button class="btn navbar__btn">
            <a href="#">Entrar</a>
        </button>
    </header>
</template>

<style>
.header {
    @apply flex items-center justify-between mx-auto z-50 relative;
    min-height: 80px;
}

.header__logo {
    width: 124px;
    height: 34px;
}

.navbar__list {
    @apply flex items-center gap-5;
}

.navbar__list__item__link {
    font-weight: 600;
    padding: 10px;
    border-bottom: 1px solid transparent;
    font-family: GGSans, sans-serif;
}

.navbar__list__item__link:hover {
    border-color: #FFF;
}

.btn.navbar__btn {
    background: #FFF;
    color: rgb(35, 39, 42);
}
.btn.navbar__btn:hover {
    color: #5865f2;
    box-shadow: 0 8px 15px rgba(0, 0, 0, .2)
}
</style>