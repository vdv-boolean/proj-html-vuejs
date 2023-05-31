<script>
export default {
	
	props: {
		img: String,
		title: String,
		date: String,
        description: String,
	},
};
</script>

<template>
    <ul>
        <li class="name">
            {{ name }}
        </li>
        <li>
            {{ title }}
        </li>
        <li>
            {{ date }}
        </li>
        <li>
            {{ description }}
        </li>
    </ul>
    
</template>

<style scoped>

    ul {
        background-color: white;
        padding: 3rem;
    }

    .name {
        font-weight: bolder;
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
    }
    
    li {
        font-weight: lighter;
        font-size: 0.8rem;
        margin-bottom: 1.5rem;
    }

    .basic-btn {
        border: 1px solid black;
    }

    .basic-btn a {
        color: black;
    }

</style>