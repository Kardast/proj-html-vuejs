<template>
  <div class="my-jumbo">

    <!-- Jumbo will contain bg img and the h1 in the middle -->
    <div class="j-wrapper">

        <P>MOVING WITHOUT THE HASSLE</P>
        <h1>WE MAKE IT SIMPLE</h1>
        <P>PROFESSIONAL SERVICE WITH QUALITY AND COSTUMER SATISFACTION</P>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyJumbo'

}
</script>

<style lang="scss">
.my-jumbo{
    width: 100%;
    background-image: url("../assets/img/avada-movers-homeherobackground-final.jpg");
    height: 620px;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;

    .j-wrapper{
        text-align: center;

        h1{
            font-size: 50px;
            margin: 15px 0;
        }

        p{
            font-size: 13px;
            color: rgb(80, 80, 80);
            font-weight: 600;
        }
    }
}

</style>
