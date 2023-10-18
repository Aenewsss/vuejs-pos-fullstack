<template>
    <h1>New component</h1>
    <span>O texto abaixo está sendo apresentado através de um v-text</span>
    <h2 v-text="randomNumber % 2 == 0 ? 'Número é par' : 'Número é ímpar'"></h2>
    <h2>O número é: {{ randomNumber }}</h2>
</template>

<script>
export default {
    name: 'NewComponent',
    data() {
        return {
            randomNumber: Math.round(Math.random() * 100 - 1)
        }
    }
}
</script>

<style scoped>
h1 {
    color: red;
}
</style>