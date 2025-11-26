<template>
<h1>For Loop Condition</h1>
<ul>
    <li v-for="item in technology" :key="item">{{ item }}</li>
</ul>
<br /><br/>

<ul>
    <li v-for="item in user" :key="item.email">Name is:{{ item.name }} and Email is:{{ item.email }}</li>
</ul>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            technology: ['java', 'vue', 'quasar', 'Html'],
            user: [{
                name: "Bhanu",
                email: 'bhanu@gmail.com'
            },
            {
                name: "Alisha",
                email: 'alisha@gmail.com'
            },
            {
                name: "Annu",
                email: 'annu@gmail.com'
            }]
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
