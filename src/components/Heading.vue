<template>
    <div>
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