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
                    isActive: "basic-btn",
                },
                {
                    name: "Premium",
                    price: "$29.99 monthly",
                    projects: "10 Projects",
                    storage: "15 GB Storage",
                    users: "Unlimited Users",
                    isActive: "basic-btn",
                },
                {
                    name: "Professional",
                    price: "$39.99 monthly",
                    projects: "15 Projects",
                    storage: "30 GB Storage",
                    users: "Unlimited Users",
                    isActive: "orange-btn",
                },
                {
                    name: "Extreme",
                    price: "$59.99 monthly",
                    projects: "Unlimited Projects",
                    storage: "Unlimited Storage",
                    users: "Unlimited Users",
                    isActive: "basic-btn",
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

      <div class="container">

        <h1>
            Our Plans
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
        </p>

        <div class="card">
            <CardFour
            v-for="(card, key) in cardFour"
            :key="card.key"
            :name="card.name"
            :price="card.price"
            :projects="card.projects"
            :storage="card.storage"
            :users="card.users"
            :isActive="card.isActive"
        />
        </div>

      </div>
        
    </section>
    
</template>

<style scoped>

    section {
        background-image: url(../../../public/img/background1.jpg);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        padding-top: 3rem;
        padding-bottom: 3rem;
        color: white;
    }

    p {
        margin-top: 2rem;
        margin-bottom: 3rem;
    }

    .card {
        display: flex;
        justify-content: space-between;
        color: black;
    }

</style>
