<script lang="ts">
export default {
    data() {
        return {
            count: 0
        }
    },
    methods: {
        increase() {
            this.count += 1;
        },
        decrease() {
            this.count -=1;
        }
    },
    mounted() {
        console.log('holis, el valor inicial del contador es ' + this.count);
    }
}
</script>

<template>
    <h1>Contador: {{ count }}</h1>
    <button @click="increase">
        Aumentar contador
    </button>
    <button @click="decrease">
        Disminuir contador
    </button>
</template>