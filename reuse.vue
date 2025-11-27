<template>
<h1>Reuse Component</h1>
<ul>
    <li v-for="item in Users" :key="item.name">

        <user :data="item"  :getData="getData" />
    </li>

</ul>
</template>

<script>
import user from './user.vue'
export default {
    name: "Home",
    components: {
        user
    },
    methods: {
        getData (name) {
            alert(name)
        }
    },
    data() {
        return {
            Users: [{
                    name: "Bhanu",
                    email: 'bhanu@gmail.com'
                },
                {
                    name: "Nisha",
                    email: 'nisha@gmail.com'
                },
                {
                    name: "Rohit",
                    email: 'rohit@gmail.com'
                },
                {
                    name: "Rahul",
                    email: 'rahul@gmail.com'
                }
            ]
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
