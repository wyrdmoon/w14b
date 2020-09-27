<template>
    <div>
<h2 @click="getJoke">{{ quote }}</h2>
<loud-joke></loud-joke>
    </div>
</template>

<script>
import axios from "axios"

    export default {
         name: "loud-joke",
    data() {
        return {
            quote: "click me!"
        }
    },
    methods: {
        getJoke: function() {
            axios.request({
                url: "https://geek-jokes.sameerkumar.website/api?format=json",
                method: "get"
            }).then((response) =>{
            console.log(response)
            this.quote = response.data
            }).catch((error) => {
                console.log(error)
            })
        }
    },
        
    }
</script>

<style lang="scss" scoped>

</style>