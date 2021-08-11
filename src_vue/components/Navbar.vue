<template>
    <nav>
        <div class="menu_item"><router-link to="/">Home</router-link></div>
        <div class="menu_item"><router-link to="/reservation">Réservation</router-link></div>
        <div class="menu_item"><router-link to="/about">About</router-link></div>
    </nav>
</template>

<script>

</script>

<style>
nav {
    display: flex;
    align-items: center;
    justify-content: left;
}

nav .menu_item {
    color: WHITE;
    padding: 20px 30px;
    position: relative;
    text-align: center;
    border-bottom: 2px solid transparent;
    display: flex;
    transition: 0.8s;
}

nav .menu_item.active,
nav .menu_item:hover {
    background-color: #444;
    border-bottom-color: YELLOW;
}

nav .menu_item a{
    color: inherit;
    text-decoration: none;
}
</style>