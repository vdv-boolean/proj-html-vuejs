<script>
export default {
	
	props: {
		icon: String,
		title: String,
		description: String,
	},
};
</script>

<template>
    <ul>
        <li> {{ icon }}</li>
        <li> {{ title }}</li>
        <li>{{ description }}</li>
    </ul>
    
</template>

<style scoped>

</style>