<template>
<h2>Student Name is :{{ name }}</h2>
</template>

    
<script>
export default {
    name: "student",
    props: {
        name:String
    }
}
</script>
