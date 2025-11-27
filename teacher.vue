<template>
    <h2>Teacher name is : {{ name }}</h2>
    </template>
    <script>
    export default {
        name: "teacher",
        props: {
            name:String
        }
    }
</script>