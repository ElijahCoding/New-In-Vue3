<template>
    <div>
        {{ posts }}
    </div>
</template>

<script>
    import axios from 'axios'

    export default {
        async setup () {
            const posts = await axios.get('https://jsonplaceholder.typicode.com/todos')

            return {
                posts
            }
        }
    }
</script>