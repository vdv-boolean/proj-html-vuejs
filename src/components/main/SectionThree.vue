<script>
    import CardThree from "./cards/CardThree.vue"
    export default {
        data() {
            return {
                cardThree: [
                    {
                        img: "public/img/case-study-gallery-1-1-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                    {
                        img: "public/img/case-study-gallery-2-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                    {
                        img: "public/img/case-study-gallery-3-1-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                    {
                        img: "public/img/case-study-gallery-4-1-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                    {
                        img: "public/img/case-study-gallery-5-1-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                    {
                        img: "public/img/case-study-gallery-6-1-800x600.jpg",
                        alt: "descrip.",
                        link: "#"
                    },
                ]
            };
        },
        components: {
            CardThree,
        }
    }
    
</script>

<template>

    <section>

        <div class="container">

            <h1>
                Our Work
            </h1>

            <p>
                Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>

            <div class="gallery">
                <CardThree 
                    v-for="(card, key) in cardThree"
                    :key="card.key"
                    :img="card.img"
                    :alt="card.alt"
                    :link="card.link"
                />
            </div>

            <button class="orange-btn">   
                <a href="">
                    View Our Work
                </a>
            </button>

        </div>

    </section>
    
</template>

<style scoped>

section {
    padding: 3rem;
}
.gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 3rem;
    margin-bottom: 3rem;
}

.gallery div {
    flex-basis: calc(33% - 10px);
}

p {
    margin-top: 2rem;
}

img {
    width: 100%;
    height: 100%;
}
</style>
