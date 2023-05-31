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
    <div class="card">
        <ul>
        <li> {{ icon }}</li>
        <li class="title">
            {{ title }}
        </li>
        <li>
            <span>
                {{ description }}
            </span>
        </li>
    </ul>
    </div>
    
    
</template>

<style scoped>
    ul {
        background-color: white;
        padding: 2rem;
    }

    li {
        margin-top: 1rem;
        margin-bottom: 1rem;
    }
   .title {
    font-size: 1.2rem;
    font-weight: bolder;
   }

   span {
    font-size: 0.8rem;
   }

</style>