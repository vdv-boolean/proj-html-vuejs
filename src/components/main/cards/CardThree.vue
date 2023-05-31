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
    </div>
     
</template>

<style scoped>
img {
    width: 100%;
    height: 100%;
}
</style>