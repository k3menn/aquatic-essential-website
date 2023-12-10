<template>
    <header class="header">
        <div class="header-logo">
            <a href="#">
                <img src="/src/assets/svg/logo.svg" alt="logo">
            </a>
        </div>
        <div class="header-menu">
            <a 
                class="header-menu--link"
                :href="element.path"
                v-for="(element, i) of menu"
                :key="i">{{element.name}}</a>
        </div>
        <div class="header-right">
            <div class="header-right--search">
                <a href="#">
                    <img src="/src/assets/svg/search.svg" alt="search">
                </a>
            </div>
            <div class="header-right--user">
                <a href="#">
                    <img src="/src/assets/svg/User.svg" alt="user">
                </a>
            </div>
            <div class="header-right--cart">
                <a href="#">
                    <img src="/src/assets/svg/shopping-bag.svg" alt="cart">
                </a>
            </div>
        </div>

    </header>
</template>

<script  setup>
import { ref } from 'vue'

const menu = [
    {
        name: "КАТАЛОГ",
        path: "/catalog"
    },
    {
        name: "КОЛЛЕКЦИИ",
        path: "/collection"
    },
    {
        name: "О НАС",
        path: "/about"
    },
    {
        name: "КОНТАКТЫ",
        path: "/contacts"
    },
    {
        name: "АКЦИИ",
        path: "/sales"
    }
]

</script>


<style scoped>
.header{
    font-family: 'Montserrat', sans-serif;
    height: 90px;
    background: #DEE0DD;
    display: flex;
    justify-content: space-between;
}
.header-logo{
    margin-top: 10px;
    margin-left: 22px;
}
.header-menu{
    display: flex;
    justify-content: center;
    align-items: center;
}

.header-menu--link{
    font-size: 22px;
    margin: 0 22px;
    color: black;
    text-decoration: none;
}

.header-menu--link:hover {
    text-decoration: underline;
}

.header-right{
    display: flex;
    align-items: center;
    justify-content: space-between 10px;
}

.header-right--search{
    margin-right: 22px;
}
.header-right--user{
    margin-right: 22px;
}
.header-right--cart{
    margin-right: 22px;
}
</style>