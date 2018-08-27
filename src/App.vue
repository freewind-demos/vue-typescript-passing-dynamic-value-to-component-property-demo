<template>
    <div>
        <input type="text" v-model="yourName" autofocus/>
        <div>{{ yourName }}</div>
        <HelloWorld v-bind:msg="yourName"/>
    </div>
</template>

<script lang="ts">
    import {Component, Vue} from 'vue-property-decorator'
    import HelloWorld from './components/HelloWorld.vue'

    @Component({
        components: {
            HelloWorld,
        },
    })
    export default class App extends Vue {
        yourName: string = ''
    }
</script>
