<template>
  <div class="my-request">

    <!-- This section will contain a background img and some text + 1 button in the middle -->   
    <div class="request-wrapper">

        <div class="request-text">

            <h2>Request A Free Quote</h2>
            <P>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptates incidunt officiis magnam qui. Cumque quibusdam error ullam. Maiores eius vitae deserunt voluptatum maxime sit laudantium itaque vero quisquam, a rem!</P>
            <a class="button" href="#">CLICK HERE</a>
        </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyRequestQuote',

}
</script>

<style lang="scss">
.my-request{
    width: 100%;
    height: 510px;
    background-image: url("../assets/img/avada-movers-request-quote-background.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .request-wrapper{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .request-text{
        text-align: center;

        span{
            font-size: 13px;
            color: rgb(80, 80, 80);
            font-weight: 600;
        }

        h2{
            color: #6abf17;
            font-size: 30px;
            margin: 15px 0;
        }

        p{
            width: 60%;
            margin: 0 auto;
            font-size: 14px;
            line-height: 25px;
            margin-bottom: 45px;
        }
        // button
        @import '../assets/button.scss';
    }
}

</style>
