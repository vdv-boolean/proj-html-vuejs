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

    span {
        color: var(--orange);
        border: 1px solid var(--orange);
        font-size: 0.5rem;
        padding: 0.2rem;
        font-weight: bolder;
    }

</style>