<template>
    <div class="hello">
        Hello, {{ msg }}!
    </div>
</template>

<script lang="ts">
    import {Component, Prop, Vue} from 'vue-property-decorator'

    @Component
    export default class HelloWorld extends Vue {
        @Prop() private msg!: string
    }
</script>

<style scoped>
    .hello {
        color: red;
    }
</style>
