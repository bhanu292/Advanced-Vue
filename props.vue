<template>
    <h1>PROPS</h1>
    <student name="Bhanu"/>
    <teacher name="Amit"/>
    </template>
    <script>
    import student from './student.vue'
    import teacher from './teacher.vue'
    export default {
        name: "Home",
        components: {
            student,
            teacher
        }
    }
</script>
<style>
h1 {
    color:orange;
}
</style>