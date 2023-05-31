<script>
    import Menu from "./Menu.vue"

    export default {
        data() {
            return {
                menuArray: [{
                    title: "Home",
                    link: "",
                    isActive: "active",
                    label: "",
                },
                {
                    title: "Who We Are",
                    link: "",
                    isActive: "",
                    label: "",
                },
                {
                    title: "What We Do",
                    link: "",
                    isActive: "",
                    label: "",
                },
                {
                    title: "Where We Work",
                    link: "",
                    isActive: "",
                    label: "",
                },
                {
                    title: "Careers",
                    link: "",
                    isActive: "",
                    label: "APPLY",
                },
                {
                    title: "News",
                    link: "",
                    isActive: "",
                    label: "",
                },
            ]
            };
        },
        components: {
               Menu, 
            }
    }

</script>

<template>

    <nav>
        <div class="left-bar">
            <img src="public/img/logo_seo_w_1x.png" alt="">
        </div>
        <div class="right-bar">
            <ul>
                <Menu
                    v-for="(link, key) in menuArray"
                    :key="link.key"
                    :title="link.title"
                    :link="link.link"
                    :isActive="link.isActive"
                    :label="link.label"
                />
            </ul>
            <button>
                Get in touch now
            </button>
        </div>
        
    </nav>
    
</template>

<style scoped>

    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 50px;
    }

    .left-bar,
    .right-bar {
        display: flex;
    }

    img {
        height: 1.5rem;
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

    
    .active {
        color: red;
    }
</style>
