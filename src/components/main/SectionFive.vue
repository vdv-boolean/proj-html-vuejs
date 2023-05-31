<script>
import CardFive from "./cards/CardFive.vue"
    export default {
        data() {
            return {
                cardFive: [{
                    img: "public/img/related-service-2-320x202.jpg",
                    title: "Why You Need a SEO Agency Now",
                    date: "November 1st, 2017",
                    description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!",
                },
                {
                    img: "public/img/related-service-2-320x202.jpg",
                    title: "SEO Tips for your Startup",
                    date: "November 1st, 2017",
                    description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!",
                },
                {
                    img: "public/img/related-service-2-320x202.jpg",
                    title: "Image Optimization For Your Site",
                    date: "November 1st, 2017",
                    description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!",

                },
            ]
            };
        },
        components: {
            CardFive,
        }
    }
</script>

<template>

    <section>
        <h1>
            Our News
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
        </p>

        <CardFive v-for="(card, key) in cardFive"
            :key="card.key"
            :img="card.img"
            :title="card.title"
            :date="card.date"
            :description="card.description"
        />

        <button class="orange-btn">   
            <a href="">
                Go to News
            </a>
        </button>
    </section>
    
</template>

<style scoped>

</style>
