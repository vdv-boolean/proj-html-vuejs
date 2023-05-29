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
                    "News",
                    "GET IN TOUCH NOW"
                ],
            };
        },
    }

</script>

<template>

    <nav>
        <div>
            Logo
            <!-- TO DO: ADD LOGO-->
        </div>
        <ul >
            <li v-for="link in linkArr">
                <a href="#">
                    {{ link }}
                </a>
            </li>
        </ul>
    </nav>
    
</template>

<style>

    nav {
        display: flex;
        justify-content: space-between;
    }

    ul {
        display: flex;
        gap: 1rem;
    }

    li {
        list-style: none;
    }

    a {
        text-decoration: none;
        color: white;
    }

</style>
