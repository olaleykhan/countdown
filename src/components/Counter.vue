<template>
    <div>
        <h1>Counter ag </h1>
        <!-- {{timer}} -->
        <!-- <h1> {{time}} </h1> -->
        <h1>{{days}} </h1>
        <h1>{{hours}} </h1>
        <h1>{{minutes}} </h1>
        <h1>{{seconds}} </h1>
    </div>
</template>

<script>
export default {
    name: "Counter",

    props: {
        // headingText: String
    },
    data(){
        return{
            // time:// Set the date we're counting down to
            time : 1728000000,

        }
    },
    computed:{
        days(){
            return Math.floor(this.time / (1000 * 60 * 60 * 24));
        },
        hours(){
            return Math.floor((this.time % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        },
        minutes(){
            return Math.floor((this.time % (1000 * 60 * 60)) / (1000 * 60));
        },
        seconds(){
           return Math.floor((this.time % (1000 * 60)) / 1000);
        }

    },
    mounted(){
        setInterval(() => {
            this.time-= 1000;
            
        }, 1000);
    }
   
}
</script>