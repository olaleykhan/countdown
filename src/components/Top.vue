<template>
    <div class="top">
        <Heading headingText="WE'RE LAUNCHING SOON"/>
        <Counter/>

    </div>
</template>

<script>
import Heading from "./Heading";
import Counter from "./Counter";
export default {
    name: "Top",
    components:{
        Heading,
        Counter,
    }
}
</script>