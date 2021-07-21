<template>
    <div class="time-card">
        <p class="display-card">{{time}} </p>
        <p class="card-name">{{name}} </p>
    </div>
</template>

<script>
export default {
    name: "TimeCard",

    props: {
        time: Number,
        name: String,
    }
}
</script>

<style scoped>

.display-card{
    color: var(--soft-red);
    font-weight: 700;
    font-size:50px;
    background-color: var(--Dark-desaturated-blue);
    width:fit-content;
    width: 80px;
    padding:20px 10px;
    border-radius: 4%;
}
@media only screen and (max-width: 800px) {
    .display-card{
        width: fit-content;
        padding: 10px 15px;
        font-size: 20px;
        margin-right: 10px;
    }
    .card-name{
        font-size: 12px;
        text-align: left;
    }
}

</style>