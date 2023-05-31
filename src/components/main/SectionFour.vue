<script>
    import CardFour from "./cards/CardFour.vue"
    export default {
        data() {
            return {
                cardFour: [{
                    name: "Standard",
                    price: "$19.99 monthly",
                    projects: "5 Projects",
                    storage: "5 GB Storage",
                    users: "Unlimited Users",
                },
                {
                    name: "Premium",
                    price: "$29.99 monthly",
                    projects: "10 Projects",
                    storage: "15 GB Storage",
                    users: "Unlimited Users",
                },
                {
                    name: "Professional",
                    price: "$39.99 monthly",
                    projects: "15 Projects",
                    storage: "30 GB Storage",
                    users: "Unlimited Users",
                },
                {
                    name: "Extreme",
                    price: "$59.99 monthly",
                    projects: "Unlimited Projects",
                    storage: "Unlimited Storage",
                    users: "Unlimited Users",
                },
            ]
            };
        },
        components: {
            CardFour
        }
    }

</script>

<template>

    <section>
        <h1>
            Our Plans
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
        </p>

        <CardFour
            v-for="(card, key) in cardFour"
            :key="card.key"
            :name="card.name"
            :price="card.price"
            :projects="card.projects"
            :storage="card.storage"
            :users="card.users"
        />
            
    </section>
    
</template>

<style scoped>

</style>
