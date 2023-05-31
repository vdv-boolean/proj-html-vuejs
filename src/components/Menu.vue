<script>

    export default {
        
        props: {
            title: String,
            link: String,
            isActive: String,
            label: String,
        },
    };

</script>

<template>

        <li >
            <button>
               <a
                    :href="link"
                    :class="isActive"
                >
                    {{ title }}
                    <span>
                        {{ label }}
                    </span>
               </a> 
            </button>
        </li>
   
</template>

<style scoped>

    .active {
        color: var(--orange);
    }

    a {
        font-size: 0.7rem;
    }

    a:hover {
        color: var(--orange);
    }

    span {
        color: var(--orange);
        font-size: 0.5rem;
        font-weight: bolder;
    }

</style>