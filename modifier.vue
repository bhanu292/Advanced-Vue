<template>
<h1>Modifiers</h1>
<input type="number" v-model.number.trim.lazy="data" />
<h2>Data is:{{ typeof (data) }}</h2>
<h2>Data is:{{ data }}</h2>
</template>

    
<script>
export default {
    name: "Home",
    data() {
        return{
            data: ''
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
