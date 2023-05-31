<script>

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

        <div
            v-for="card in cardFour"
        >
            <ul>
                <li>
                    {{ card.name }}
                </li>
                <li>
                    {{ card.price }}
                </li>
                <li>
                    {{ card.projects }}
                </li>
                <li>
                    {{ card.storage }}
                </li>
                <li>
                    {{ card.users }}
                </li>
                <button>
                    <a href="">Start TODAY</a>
                </button>
            </ul>
        </div>
    </section>
    
</template>

<style scoped>

</style>
