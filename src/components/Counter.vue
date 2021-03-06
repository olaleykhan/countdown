<template>
    <div class="counter">
        <!-- <p>{{TimeCard}} </p> -->
        <TimeCard name="Days" :time="days"/>
        <TimeCard name="Hours" :time="hours"/>
        <TimeCard name="Minutes" :time="minutes"/>
        <TimeCard name="Seconds" :time="seconds"/>
        <!-- <TimeCard name="Seconds" :time="seconds"/> -->
    </div>
</template>

<script>
import TimeCard from "./TimeCard";
export default {
    name: "Counter",
    components:{
        TimeCard
    },

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

<style scoped>
.counter{
    display:flex;
    justify-content:space-between;
    width: 40vw;
    margin: 15vh auto;
}
</style>