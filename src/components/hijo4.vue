<template>
    <div>
        <h2>hijo 4</h2>
        <h4>esta es la info del hijo 3</h4>
        <h6>{{informacion}}</h6>
        <hr>
    </div>
</template>
<script>
import {eventBus} from '../main'
export default {
    data(){
        return{
            informacion:""
        }
    },
    created() {
        eventBus.$on("pasar",(data)=>{
            return this.informacion = data
        })
    },
}
</script>
<style scoped>
</style>