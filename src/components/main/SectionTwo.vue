<script>
    import CardTwo from "./cards/CardTwo.vue"
    export default {
        data() {
            return {
                cardTwo: [
                    {
                        icon: "iconsrc",
                        title: "Google SEO",
                        description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Est hic alias voluptates, at debitis dicta deleniti? Tempora nihil debitis! Tempora nihil debitis!Tempora nihil debitis!",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "Brand Strategy",
                        description: "Assumenda asperiores dolorem autem quas obcaecati. Nobis quas culpa saepe eaque quaerat! Cum quibusdam rerum delectus temporibus neque.",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "Local SEO",
                        description: "Dolor voluptatem pariatur aliquam quam atque iusto saepe rerum et, tempora, optio iure! Sit molestias pariatur, nesciunt quae earum eius.",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "SEO Analysis",
                        description: "Dolor voluptatem pariatur aliquam quam atque iusto saepe rerum et, tempora, optio iure! Sit molestias pariatur, nesciunt quae earum eius.",
                        link: "#"
                    },
                ]
            };
        },
        components: {
            CardTwo,
        }
    }
    
</script>

<template>

    <section>
        
        <div class="container">

            <h1>
                See Our Top Notch Services
            </h1>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
            </p>

            <div class="card">
                <CardTwo 
                    v-for="card in cardTwo"
                    :key="card.key"
                    :icon="card.icon"
                    :title="card.title"
                    :description="card.description"
                    :link="card.link"
                />
            </div>

        </div>

    </section>
    
</template>

<style scoped>

    section {
        background-color: rgb(1, 1, 82);
        background-image: url(../../../public/img/pattern_background.png);
        background-size: contain;
        background-repeat: no-repeat;
        color: white;
        padding-top: 3rem;
        padding-bottom: 3rem;
    }

    p {
        margin-top: 2rem;
        margin-bottom: 2rem;
    }

    .card {
        display: flex;
        gap: 2rem;
    }

</style>
