<script>

    import CardOne from "./cards/CardOne.vue"

    export default {
        data() {
            return {
                cardOne: [{
                    icon: "iconsrc",
                    title: "Estabilish Goals",
                    description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Est hic alias voluptates, at debitis dicta deleniti? Tempora nihil debitis, quas animi beatae obcaecati ex laborum vel neque, iusto modi corporis!",
                },
                {
                    icon: "iconsrc",
                    title: "Work With a Team",
                    description: "Assumenda asperiores dolorem autem quas obcaecati. Nobis quas culpa saepe eaque quaerat! Cum quibusdam rerum delectus temporibus neque aliquid illo, inventore optio. Fugit incidunt, unde vero veniam aliquid neque rerum.",
                },
                {
                    icon: "iconsrc",
                    title: "Gets Results",
                    description: "Dolor voluptatem pariatur aliquam quam atque iusto saepe rerum et, tempora, optio iure! Sit molestias pariatur, nesciunt quae earum eius officiis aliquam nam laudantium, ut sequi. Quibusdam minus sed doloribus.",
                },
            ]
            };
            
        },
        components: {
        CardOne,
        }
    }

</script>

<template>

    <section>

        <div class="container">
            <h1>
                Meet The New Agency SEO Template From The Avada Team
             </h1>

            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!            
            </p>

            <div class="card">
                <CardOne 
                    v-for="card in cardOne"
                    :key="card.key"
                    :icon="card.icon"
                    :title="card.title"
                    :description="card.description"
                />
            </div>

            <img src="public/img/agency-seo-desk-front-1200x570.jpg" alt="">

        </div>
        
    </section>
    
</template>

<style scoped>

    section {
        background-color: var(--white);
        padding-top: 3rem;
    }

    p {
        margin-top: 3rem;
        margin-bottom: 3rem;
    }

    img {
        width: 100%;
    }

    .card {
        display: flex;
        flex-wrap: flex;
        gap: 1rem;
    }

</style>
