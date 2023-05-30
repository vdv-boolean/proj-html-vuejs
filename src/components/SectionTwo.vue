<script>

    export default {
        data() {
            return {
                cardTwo: [
                    {
                        icon: "iconsrc",
                        title: "Google SEO",
                        description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Est hic alias voluptates, at debitis dicta deleniti? Tempora nihil debitis, quas animi beatae obcaecati ex laborum vel neque, iusto modi corporis!",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "Brand Strategy",
                        description: "Assumenda asperiores dolorem autem quas obcaecati. Nobis quas culpa saepe eaque quaerat! Cum quibusdam rerum delectus temporibus neque aliquid illo, inventore optio. Fugit incidunt, unde vero veniam aliquid neque rerum.",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "Local SEO",
                        description: "Dolor voluptatem pariatur aliquam quam atque iusto saepe rerum et, tempora, optio iure! Sit molestias pariatur, nesciunt quae earum eius officiis aliquam nam laudantium, ut sequi. Quibusdam minus sed doloribus.",
                        link: "#"
                    },
                    {
                        icon: "iconsrc",
                        title: "SEO Analysis",
                        description: "Dolor voluptatem pariatur aliquam quam atque iusto saepe rerum et, tempora, optio iure! Sit molestias pariatur, nesciunt quae earum eius officiis aliquam nam laudantium, ut sequi. Quibusdam minus sed doloribus.",
                        link: "#"
                    },
                ]
            };
        },
    }
    
</script>

<template>

    <section>
        <h1>
            See Our Top Notch Services
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
        </p>

        <ul>
            <li v-for="card in cardTwo">
                <div>{{ card.icon }}</div>
                <div>{{ card.title }}</div>
                <div>{{ card.description }}</div>
                <button>
                    <a 
                        :href="card.link"
                    >   
                        Read More...
                    </a>
                </button>
            </li>
        </ul>

    </section>
    
</template>

<style scoped>

</style>
