<template>
  <div class="my-award">

    <!-- This section will contain e blue stripe  on the top and some text + 1 button in the middle -->
    <div class="o-quote">
        <font-awesome-icon icon="fa-regular fa-paper-plane" />
        <p>GET A FREE QUOTE ONLINE NOW!</p>
    </div>
    
    <div class="award-wrapper">

        <div class="award-text">

            <span>HEADACHE FREE</span>
            <h2>Award Winning <br> Moving Company</h2>
            <P>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptates incidunt officiis magnam qui. Cumque quibusdam error ullam. Maiores eius vitae deserunt voluptatum maxime sit laudantium itaque vero quisquam, a rem!</P>
            <a class="button" href="#">READ OUR TESTIMONIALS</a>
        </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyAwardSection',

}
</script>

<style lang="scss">
.my-award{
    width: 100%;
    height: 510px;
    background-color: #f8f9fd;

    .o-quote{
        width: 100%;
        height: 110px;
        background-color: #1775bf;
        display: flex;
        justify-content: center;
        align-items: center;

        .fa-paper-plane{
            color: white;
            margin-right: 10px
        }

        p{
            color: white;
        }
    }
    .award-wrapper{
        width: 100%;
        height: calc(100% - 110px);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .award-text{
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
            width: 40%;
            margin: 0 auto;
            font-size: 14px;
            line-height: 25px;
            margin-bottom: 25px;
        }
        // button
        @import '../assets/button.scss';
    }
}

</style>
