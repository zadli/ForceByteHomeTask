<script setup>

const onClick = () => {
    document.getElementsByClassName("burger-menu__expanded")[0].classList.toggle("active");
}
const menuClick = (link, num) => {
    if (link === window.location.pathname) {
        document.getElementsByClassName("submenu")[num].classList.toggle("active");
        document.getElementsByTagName("img")[num + 2].classList.toggle("rotated")
    } else {
        window.location.href = link
    }
}
</script>

<template>
    <div class="header">
        <div class="header-logo">
            <router-link to="/">
                <img src="@/assets/logo.svg" alt="logo">
            </router-link>
        </div>
        <div class="burger-menu" v-on:click="onClick()">
            <img src="@/assets/burger.svg" alt="logo">
        </div>
    </div>
    <div class="burger-menu__expanded">
        <svg v-on:click="onClick()" xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 22 22"
            fill="none">
            <path d="M22 2.2L19.8 0L11 8.8L2.2 0L0 2.2L8.8 11L0 19.8L2.2 22L11 13.2L19.8 22L22 19.8L13.2 11L22 2.2Z"
                fill="white" />
        </svg>
        <div class="menu">
            <div class="menu__item">
                <div class="menu__title" v-on:click="menuClick('/', 0)">
                    <span>Index</span>
                    <img src="@/assets/arrow.svg" />
                </div>
                <div class="submenu">
                    <div class="submenu__item">
                        <span>Menu</span>
                    </div>
                    <div class="submenu__item">
                        <span>Name</span>
                    </div>
                    <div class="submenu__item">
                        <span>About</span>
                    </div>
                    <div class="submenu__item">
                        <span>Footer</span>
                    </div>
                </div>
            </div>
            <div class="menu__item">
                <div class="menu__title" v-on:click="menuClick('/contact', 1)">
                    <span>Contact</span>
                    <img src="@/assets/arrow.svg" />
                </div>
                <div class="submenu">
                    <div class="submenu__item">
                        <span>Menu</span>
                    </div>
                    <div class="submenu__item">
                        <span>Name</span>
                    </div>
                    <div class="submenu__item">
                        <span>About</span>
                    </div>
                    <div class="submenu__item">
                        <span>Footer</span>
                    </div>
                </div>
            </div>
            <div class="menu__item">
                <div class="menu__title" v-on:click="menuClick('/blog', 2)">
                    <span>Blog</span>
                    <img src="@/assets/arrow.svg" />
                </div>
                <div class="submenu">
                    <div class="submenu__item">
                        <span>Menu</span>
                    </div>
                    <div class="submenu__item">
                        <span>Name</span>
                    </div>
                    <div class="submenu__item">
                        <span>About</span>
                    </div>
                    <div class="submenu__item">
                        <span>Footer</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.burger-menu__expanded {
    width: 30%;
    height: 100%;
    transform: translateX(100%);
    transition: all 0.3s ease;
    position: fixed;
    top: 0;
    right: 0;
    background: #5A98D0;
    border-radius: 50px 0px 0px 0px;
}

.burger-menu__expanded.active {
    transform: translateX(0);
}

.burger-menu__expanded svg {
    position: absolute;
    right: 18px;
    top: 22px;
}

.burger-menu__expanded .menu {
    display: flex;
    flex-direction: column;
    overflow: auto;
    width: calc(100% - 60px);
    height: 85%;
    margin-top: 100px;
    margin-left: 50px;
}

.burger-menu__expanded .menu img {
    margin-left: 16px;
    transform: rotate(180deg);
    transition: all 0.3s ease;
}

.burger-menu__expanded .menu img.rotated {
    transform: rotate(0);
}

.burger-menu__expanded .menu .menu__item {
    display: flex;
    flex-direction: column;
    margin-bottom: 32px;
}

.burger-menu__expanded .menu .menu__item .menu__title {
    display: flex;
}

.burger-menu__expanded .menu .menu__item span {
    font-size: 1.5rem;
    color: white;
}

.burger-menu__expanded .menu .menu__item .submenu {
    opacity: 0;
    visibility: collapse;
    height: 0;
    transition: all 0.3s ease;
}

.burger-menu__expanded .menu .menu__item .submenu.active {
    opacity: 1;
    visibility: visible;
    height: auto;
}

.burger-menu__expanded .menu .menu__item .submenu .submenu__item {
    margin-top: 24px;
    opacity: 0.7;
}

.burger-menu__expanded .menu .menu__item .submenu .submenu__item span {
    font-size: 1rem;
    color: white;
}

.header {
    position: fixed;
    top: 0;
    height: 96px;
    width: 100%;
    background-color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    align-content: center;
}

.header img {
    margin-right: 64px;
    margin-left: 64px;
}
</style>