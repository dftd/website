<template>
    <div class="page-projects">
        <router-link to="/" class="close"></router-link>
        <div class="container">
            <div class="project">
                <h2>
                    <a href="//free-classifieds.co.uk" target="_blank">FreeClassifieds UK</a>
                    <span class="badges"><span>HTML/CSS/JS</span><span>PHP</span></span>
                </h2>
                <p>Custom Osclass theme (Bootstrap) & custom Osclass plugins (profile picture, captcha, moderation system and more).</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//kanesex.com" target="_blank">Kanesex</a>
                    <span class="badges"><span>HTML/CSS/JS</span><span>PHP</span></span>
                </h2>
                <p>Custom Osclass plugins (paysafecard payments, social network system).</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//exportmaschinen.de" target="_blank">ExportMaschinen</a>
                    <span class="badges"><span>HTML/CSS/JS</span><span>PHP</span></span>
                </h2>
                <p>Custom Osclass plugins (filterable map page for ads, ad attributes).</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//farmernear.me" target="_blank">Farmer Near Me</a>
                    <span class="badges"><span>HTML/CSS/JS</span><span>PHP</span><span>Java</span></span>
                </h2>
                <p>Custom Osclass plugins (e-commerce, nearby ads - geolocation) & web-view mobile application.</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//mmx-afroonet.co.zw" target="_blank">MMX Afroonet</a>
                    <span class="badges"><span>HTML/CSS/JS</span><span>PHP</span></span>
                </h2>
                <p>Custom Osclass plugins (paynow payments).</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//top.gg/bot/753982465261174847" target="_blank">ApplyBot</a>
                    <span class="badges"><span>node.js</span><span>Discord</span></span></span>
                </h2>
                <p>Discord application bot built with discord.js, serving in 1500+ servers.</p>
            </div>
            <div class="project">
                <h2>
                    <a href="//cod1x.eu" target="_blank">CoDExtended Client</a>
                    <span class="badges"><span>C/C++</span><span>Reverse Engineering</span></span>
                </h2>
                <p>Clientside modification for Call of Duty 1.1 with bugfixes & new features.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Projects',
    data () {
        return {
            stuff: ''
        }
    }
}
</script>

<style scoped>
.close {
    position: absolute;
    top: 4rem;
    right: 4rem;
    width: 4rem;
    height: 4rem;
}
.close:before, .close:after {
    content: "";
    transform: rotate(-45deg);
    position: absolute;
    top: 50%;
    left: 50%;
    margin-top: -5px;
    margin-left: -25px;
    display: block;
    height: .8rem;
    width: 4rem;
    background-color: #fff;
    transition: all 0.25s ease-out;
}
.close:after {
    transform: rotate(-135deg);
}
.close:hover:before, .close:hover:after {
    transform: rotate(0deg);
}

.container {
    display: flex;
    justify-content: center;
    max-width: 960px;
    min-height: 100vh;
    margin-left: auto;
    margin-right: auto;
    padding: 3rem;
    flex-direction: column;
}

.project {
    margin-bottom: 3rem;
}
.project h2 {
    margin-bottom: 1rem;
}

.badges span {
    background: #f05051;
    border-radius: .25rem;
    padding: .25rem .5rem;
    margin: 0 .25rem;
    font-size: .75rem;
}

@media (max-width: 576px) {
    .close {
        top: 1rem;
        right: 1rem;
        width: 3rem;
        height: 3rem;
    }
    .close:before, .close:after {
        height: .5rem;
        width: 2.5rem;
    }

    .badges {
        display: block;
        margin-left: -3px;
    }
}
</style>