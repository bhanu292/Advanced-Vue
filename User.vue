<template>
<div>
    <h3>Bhanu</h3>
    <h3>Nishu</h3>
    <h3 v-bind="$attrs">Alisha</h3>
    <h3>{{ data }}</h3>
</div>
</template>

<script>
export default {
    name: "User",
    inheritAttrs: false,
    props:{
        data:String
    }
}
</script>
