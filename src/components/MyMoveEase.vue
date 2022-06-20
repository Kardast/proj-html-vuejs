<template>
  <div class="my-move-ease">

    <!-- Jumbo will contain bg img and the h1 in the middle -->
    <div class="move-wrapper">
      <div class="move-bg-wrapper">
        
        <span>WE REMOVE THE HEADACHE FROM MOVING</span>
        <h2>MOVE WITH EASE</h2>
        <p>
          With our super simple service we can take you from getting a quote, <br>
          right through to being in your new home with all of your belongings <br>
          securely packed and safely delivered, even in the rooms of your choice.
        </p>
        <a class="button" href="#">GET A FREE QUOTE NOW</a>
      </div>

    </div>
  </div>
</template>

<script>


export default {
  name: 'MyMoveEase'

}
</script>

<style lang="scss">
.my-move-ease{
  width: 100%;
  background-image: url("../assets/img/avada-movers-movewithease-background-new.jpg");
  height: 750px;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;

  .move-wrapper{
    text-align: center;
    color: white;
    // button
    @import '../assets/button.scss';
    background-color: #5aa511;
    padding: 10px;
    margin-left: 30%;

    .move-bg-wrapper{
      background-color: #6abf17;
      padding: 25px 30px 40px 30px;

      span{
        font-size: 12px;
        font-weight: 600;
      }

      h2{
        font-size: 35px;
        margin: 10px auto 25px auto;
        border-bottom: 2px solid #92f235;
        padding-bottom: 15px;
        width: 330px;
      }

      p{
        font-size: 12px;
        font-weight: 600;
        line-height: 25px;
        margin-bottom: 30px;
      }
    }
  }
}

</style>
