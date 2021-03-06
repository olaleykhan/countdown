<template>
    <div class="heading">
        <h1>{{headingText}} </h1>
    </div>
</template>

<script>
export default {
    name: "Heading",

    props: {
        headingText: String
    }
}
</script>

<style scoped>
.heading {
    padding-top:100px;
    font-size:14px;
    font-weight:700;
}


</style>