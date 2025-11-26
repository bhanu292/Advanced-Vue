<template>
    <h1>Get Checkbox and Radio Button values</h1>
    <h3>Technology</h3>
    <label for="java">Java</label>
    <input type="checkbox" value="java" v-model="technology" id="java" />

    <label for="javascript">Javascript</label>
    <input type="checkbox" value="javascript" v-model="technology" id="javascript" />
    
    <label for="vue">VUE</label>
    <input type="checkbox" value="vue" v-model="technology" id="vue" />

    <br /><br />
    <h3>Who I Am</h3>
    
    <label for="student">Student</label>
    <input type="radio" value="student" name="who" v-model="who" id="student" />
    
    <label for="developer">Developer</label>
    <input type="radio" value="developer" name="who" v-model="who" id="developer" />
    
    <h4>Selected Technology:{{ technology }}</h4>
       <h4>I Am A:{{ who }}</h4>
    
    </template>

    <script>
    export default {
        name: "Home",
        data () {
            return {
                technology:[],
                who:null
            }
        }
    }
</script>

<style>
h1 {
    color:orange;
}
</style>