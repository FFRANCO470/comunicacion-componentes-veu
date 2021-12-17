<template>
    <div>
        <h2>hijo 2</h2>
        <h4>envia al padre</h4>
        <button @click="pasar()" >hijo2</button>
        <hr>
    </div>
</template>
<script>
export default {
    data(){
        return{
            mensaje:"info del hijo al padre"
        }
    },
    methods: {
        pasar(){
            this.$emit("recibirHijo",this.mensaje)
        }
    },
}
</script>
<style scoped>
</style>