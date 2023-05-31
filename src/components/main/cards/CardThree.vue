<script>
export default {
	
	props: {
		img: String,
		alt: String,
        link: String,
	},
};
</script>

<template>
    <div>
        <img 
        :src="img"
        :alt="alt"
        > 
        <button>
            <a :href="link">link</a>
        </button>
    </div>

     
</template>

<style scoped>

div {
    position: relative;
}

img {
    width: 100%;
    height: 100%;
}

button {
    width: 100%;
    height:100%;
    position: absolute;
    top: 0;
    left: 0;
    opacity: 0%;
    border-radius: 0%;
}

button:hover {
    opacity: 100%;
    background: linear-gradient(var(--violet), transparent);
}

</style>