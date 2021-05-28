<template>
    <div id="app">
        <transition name="fade" mode="out-in">
            <router-view/>
        </transition>
    </div>
</template>

<script>
export default {
    name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;400;500&display=swap');

* {
    box-sizing: border-box;
    margin-block-start: 0em;
    margin-block-end: 0em;
}

body {
    margin: 0;
    padding: 0;
}

#app {
    font-family: 'Montserrat', sans-serif;
    background: #2d3436;
    color: #fff;
}

a {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
}

.red {
    color: #f05051
}

.fade-enter-active, .fade-leave-active {
    transition: opacity 0.5s ease;
}
.fade-enter-from, .fade-leave-to {
    opacity: 0;
}
</style>