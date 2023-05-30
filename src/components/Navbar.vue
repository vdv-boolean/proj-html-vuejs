<script>

    export default {
        data() {
            return {
                linkArr: [
                    "Home",
                    "Who We Are",
                    "What We Do",
                    "Where We Work",
                    "Careers",
                    "News"
                ],
            };
        },
    }

</script>

<template>

    <nav>
        <div class="left-bar">
            <img src="public/img/logo_seo_1x.png" alt="">
        </div>
        <div class="right-bar">
            <ul>
                <li v-for="link in linkArr">
                    <a href="#">
                        {{ link }}
                    </a>
                </li>
            </ul>
            <button>
                Get in touch now
            </button>
        </div>
        
    </nav>
    
</template>

<style>

    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 50px;
    }

    .right-bar {
        display: flex;
    }

    ul {
        display: flex;
        gap: 1rem;
        padding-inline: 1rem;
    }

    li {
        list-style: none;
    }

    a {
        text-decoration: none;
        color: white;
    }

</style>
