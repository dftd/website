<template>
    <div class="page-home">
        <div class="container">
            <div class="col logo">
                <img src="../assets/logo.svg">
                <h1>defected<span class="red">.</span>dev</h1>
            </div>
            <div class="col content">
                <h2>Hey there! {{ emoji }}</h2>
                <p class="bio">
                    I am a freelance Web Developer based in Croatia.
                    <br>
                    Technologies that I worked with include: HTML/CSS/JS, node.js, PHP, MySQL, MongoDB, Wordpress, Joomla and Osclass.
                </p>
                <div class="links">
                    <a class="projects"><router-link to="/projects">view projects</router-link></a>
                    <a href="mailto:info@defected.dev" target="_blank">
                        <img src="../assets/icon-mail.svg"> info<span class="red">@</span>defected<span class="red">.</span>dev
                    </a>
                    <a href="//github.com/dftd" target="_blank">
                        <img src="../assets/icon-github.svg"> github<span class="red">.</span>com<span class="red">/</span>dftd
                    </a>
                </div>
            </div>
        </div>    
    </div>
</template>

<script>
export default {
    name: 'Home',
    data () {
        return {
            emoji: ''
        }
    },
    created() {
        let emojis = ['👋', '👋🏻', '👋🏼', '👋🏽', '👋🏾', '👋🏿'];
        this.emoji = emojis[ Math.floor(Math.random() * emojis.length) ];
    },
}
</script>

<style scoped>
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 960px;
    min-height: 100vh;
    margin-left: auto;
    margin-right: auto;
}

.col {
    padding: 3rem;
}

.logo {
    width: 25%;
    text-align: center;
}
.logo img {
    width: 8rem;
}
.logo h1 {
    font-size: 1.25rem;
}

.content h2 {
    font-size: 2rem;
    margin-bottom: 1.75rem;
}
.content .bio {
    margin-bottom: 1.25rem;
}
.content .links .projects {
    background: #f05051;
    padding: .25rem .5rem;
    border-radius: .25rem;
}
.content .links a:not(:last-of-type) {
    margin-right: 1rem
}
.content .links img {
    height: 1.19rem;
    vertical-align: bottom;
}

@media (max-width: 768px) {
    .container {
        flex-direction: column;
        text-align: center;
    }

    .logo {
        width: 100%;
        padding-bottom: 0;
    }

    .content .links {
        margin-top: 2rem;
    }
    .content .links a {
        display: block;
        margin: 1rem 0;
    }
    .content .links a:not(:last-of-type) {
        margin-right: 0;
    }
}
</style>