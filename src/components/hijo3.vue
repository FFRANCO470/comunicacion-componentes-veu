<template>
    <div>
        <h2>hijo 3</h2>
        <button @click="emitirInfo()" >hijo 3</button>
        <hr>
    </div>
</template>
<script>
import {eventBus} from '../main'
export default {
    methods: {
        emitirInfo(){
            eventBus.$emit("pasar","esa es info de hijo 3 a hijo 4")
        }
    },
}
</script>
<style scoped>
</style>