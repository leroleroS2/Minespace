<template>
    <section>
        <slider-goiaba :slides="goiaba"/>

        <!-- <div v-for="(item, index) in goiaba" :key="index">
            <h1>qualquer coisa</h1>
            <p>{{item.title}}</p>
            <img :src="item.url" alt="">
        </div> -->
    </section>
</template>

<script>
    import axios from "axios"

    export default{
        data(){
            return{

                goiaba : ""

            }
        },

        mounted(){
            this.getAPI()
        },

        methods:{
            async getAPI(){
                const {data} = await axios.get("https://jsonplaceholder.typicode.com/photos?_limit=2&_start=2")

                console.log(data)
                this.goiaba = data
            }
        }
    }
</script>