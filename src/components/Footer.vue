<template>
<div class="footer">
     <div class="footer-icons">
         <img class="footer-icon" src="../assets/icon-facebook.svg" alt="">
         <img class="footer-icon" src="../assets/icon-pinterest.svg" alt="">
         <img class="footer-icon" src="../assets/icon-instagram.svg" alt="">
     </div>
</div>
   
</template>

<script>
export default {
    name: 'Foooter',
    
    
}
</script>

<style scoped>
.footer{
    background-image: url("../assets/pattern-hills.svg");
    background-repeat: no-repeat;
    /* height: 30vh; */
    position:absolute;
    bottom: 0;
    left: 0;
    right: 0;
    padding-top: 10vh;
    padding-bottom:10vh;
}
.footer-icons{
    display: flex;
    justify-content: space-between;
    width:150px;
    margin: 20px auto;
    /* color: var(--grayish-blue); */
    /* color: red; */
}
.footer-icons > img{
    color:red;
    /* background-color: blue; */
}

</style>