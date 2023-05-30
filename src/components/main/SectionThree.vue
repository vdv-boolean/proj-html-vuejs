<script>

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

        <div v-for="(card, key) in cardThree"
        :key="key">
            
            
            <img 
                 
                :src="card.img"
                :alt="card.alt"
            >
        </div>

        <button>   
            View Our Work
        </button>
    </section>
    
</template>

<style scoped>

</style>
