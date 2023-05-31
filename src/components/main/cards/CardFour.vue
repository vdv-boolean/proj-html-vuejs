<script>
export default {
	
	props: {
		name: String,
		price: String,
		projects: String,
        storage: String,
        users: String,
	},
};
</script>

<template>
    <ul>
        <li>
            {{ name }}
        </li>
        <li>
            {{ price }}
        </li>
        <li>
            {{ projects }}
        </li>
        <li>
            {{ storage }}
        </li>
        <li>
            {{ users }}
        </li>
        <button>
            <a href="">Start TODAY</a>
        </button>
    </ul>
    
</template>

<style scoped>

</style>