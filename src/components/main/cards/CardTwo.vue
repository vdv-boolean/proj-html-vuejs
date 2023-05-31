<script>
export default {
	
	props: {
		icon: String,
		title: String,
		description: String,
        link: String,
	},
};
</script>

<template>
    <ul>
        <li>
            {{ icon }}
        </li>
        <li>
            {{ title }}
        </li>
        <li>
            {{ description }}
        </li>
        <li>
            <button>
                <a 
                    :href="link"
                >   
                    Read More...
                </a>
            </button>
        </li>
    </ul>
    
</template>

<style scoped>

</style>