<template>
    <p>{{ text }}</p>
</template>

<script>
    export default {
        props: {
            text: {
                required: true,
                type: String
            }
        },

        setup (props) {
            console.log(props.text)
        }
    }
</script>