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
        <h1>
            Our Work
        </h1>

        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque ipsum consectetur autem ipsam!
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

        <button>   
            View Our Work
        </button>
    </section>
    
</template>

<style scoped>

.gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

.gallery div {
    flex-basis: calc(33% - 10px);
}

img {
    width: 100%;
    height: 100%;
}
</style>
