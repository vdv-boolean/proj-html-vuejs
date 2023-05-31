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
            <i class="fa-brands fa-google">hgfd</i>
        </li>
        <li class="title">
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
                    Read More >
                </a>
            </button>
        </li>
    </ul>
    
</template>

<style scoped>

    ul {
        background-color: var(--blue);
        padding: 2rem;
    }

    ul:hover {
        box-shadow: inset 0px 0px 0px 12px var(--violet)
    }
    .title {
        font-weight: bolder;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }

    a {
        color: var(--orange);
    }

</style>