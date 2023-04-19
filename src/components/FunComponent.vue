<template>
    <div>
    <button @click="changeColor">Change color</button>
    <div class="color-card">
        <h1 v-for="(secret, i) in secrets" :key="i" @click="changeColorOfp" class="colorP" >{{ secret }}</h1>
    </div>
    </div>
    
</template>

<script>
export default {
        data() {
            return {
                secrets: ['hey','hello','good-Morning']
            }
        },
    methods: {
        changeColor: function (){
            let getDiv = document.querySelector(`.color-card`)
            getDiv[`style`][`backgroundColor`]=`lightblue`
        }, 
        changeColorOfp: function (details) {
            details[`target`][`style`][`color`]=`pink`

        } 
       }
    }
</script>

<style scoped>
div{
    
    min-height: 80vh;
}
button{
    background: red;
    width: 200px;
    padding: 10px;
    border: none;
}
.color-card{
    min-height: 40vh;
    border: 3px solid red;
}
</style>