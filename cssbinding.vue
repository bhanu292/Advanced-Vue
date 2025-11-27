<template>
<h1>CSS Binding</h1>
<h2 :class="applystyle">Home Component</h2>
<button v-on:click="colorful=!colorful">Apply Style</button>
</template>

    
<script>
export default {
    name: "Home",
    data () {
        return {
            colorful:false
        }
    },
    computed: {
        applystyle () {
            return {
                green:this.colorful,
                err:true,
                other:true
            }
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
.green {
    background-color: green;
    width:200px;
    padding:10px;
}
.err {
    color:rgb(227, 143, 16);
}
.other {
    font-size:30px;
}
</style>
