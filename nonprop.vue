<template>
<h1>NONPROPS</h1>
<User data="some data" id="user.cmp" />
</template>

    
<script>
import User from './User.vue';
export default {
    name: "Home",
    components:{
        User
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
