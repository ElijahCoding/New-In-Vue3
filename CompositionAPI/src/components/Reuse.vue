<template>
    <div>
        {{ x }} {{ y }}
    </div>
</template>

<script>
    import { useMousePosition } from '../mouse'
    export default {
        setup () {
            const { x, y } = useMousePosition()

            return {
                x, y
            }
        }
    }
</script>