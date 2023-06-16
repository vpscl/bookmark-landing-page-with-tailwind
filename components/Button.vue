<template>
    <button type="button" :class="`btn py-3 px-6 rounded-md transition duration-300
    ${btnClass} ${shadow && 'shadow-md'} ${uppercase && 'uppercase'}
    ${purple && 'bg-bookmark-purple text-white hover:bg-indigo-600'}
    ${white && 'bg-bookmark-white text-black hover:bg-gray-200'}`">
        {{ title }}
    </button>
</template>

<script>
    export default {
        props: {
            shadow: {
                type: Boolean,
                default: false
            },
            btnClass: {
                type: String
            },
            title: {
                type: String,
            },
            uppercase: {
                type: Boolean,
                default: false
            },
            purple: {
                type: Boolean,
                default: false
            },
            white: {
                type: Boolean,
                default: false
            }
        }
    }
</script> 