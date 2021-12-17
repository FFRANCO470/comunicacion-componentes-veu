<template>
    <div>
        <h2>hijo 1</h2>
        <h4>recibe del padre</h4>
        <h6>aca se ve lo que envia : {{recibiendo}}</h6>
        <hr>
    </div>
</template>
<script>
export default {
    props:['recibiendo']
}
</script>
<style scoped>
</style>