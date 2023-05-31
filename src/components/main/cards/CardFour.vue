<script>
export default {
	
	props: {
		name: String,
		price: String,
		projects: String,
        storage: String,
        users: String,
        isActive: String,
	},
};
</script>

<template>
    <ul>
        <li class="name">
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
        <button :class="isActive">
            <a href="">
                Start Today
            </a>
        </button>
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