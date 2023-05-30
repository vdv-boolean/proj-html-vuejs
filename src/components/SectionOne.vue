<script>

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
}

</script>

<template>

    <section>
        <h1>
            Meet The New Agency SEO Template From The Avada Team
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!            
        </p>

        <ul>
            <li v-for="card in cardOne">
                <div>{{ card.icon }}</div>
                <div>{{ card.title }}</div>
                <div>{{ card.description }}</div>
            </li>
        </ul>
        
        <img src="../img/agency-seo-desk-front-1200x570.jpg" alt="">
    </section>
    
</template>

<style scoped>

</style>
