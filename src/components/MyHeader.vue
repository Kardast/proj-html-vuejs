<template>
  <div class="my-header">

    <!-- Header will be divided in two parts -->
    <div class="h-socials">

      <div class="htop-wrapper">

        <div class="telephone">

          <p>
            <font-awesome-icon icon="fa-solid fa-phone-flip" /> 
            Call us for a Free Quote: 1.800.55.6789
          </p>
        </div>

        <!-- My Socials -->
        <ul class="socials">

          <li v-for="(item, i) in headerSocial" :key="i">
            <a href="#">
              <font-awesome-icon :icon="item.social" />
            </a>
          </li>
        </ul>
      </div>
    </div>

    <div class="h-links">

      <div class="hbottom-wrapper">

        <div class="logo">
          
          <img src="../assets/img/avada-movers-logo.png" alt="">
        </div>

        <!-- My Links -->
        <ul class="links">

          <li v-for="(item, k) in headerLinks" :key="k">
            <a href="#">
              {{item.link}}
            </a>
          </li>
        </ul>

          <div class="button-wrapper">

            <a class="button" href="#">FREE QUOTE</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyHeader',

  props: {
    headerSocial: Array,
    headerLinks: Array
  }

}
</script>

<style lang="scss">
.my-header{
  width: 100%;
  height: 150px;
  background-color: rgba(255, 255, 255, 0.39);

  .h-socials{
    width: 100%;
    height: 50px;
    background-color: #6abf17;

    .htop-wrapper{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      display: flex;

      .telephone{
        width: 50%;
        display: flex;
        align-items: center;
        color: white;
      }

      .socials{
        width: 50%;
        display: flex;
        align-items: center;
        justify-content: end;
        list-style: none;
        
        li{
          margin: 0 15px;

          a{
            text-decoration: none;
            color: white;
          }
        }

      }
    }
  }

  .h-links{
    width: 100%;
    height: 100px;

    .hbottom-wrapper{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      display: flex;

      .logo{
        width: 30%;
        display: flex;
        align-items: center;
      }

      .links{
        width: 70%;
        display: flex;
        align-items: center;
        justify-content: end;
        list-style: none;

        li{
          margin: 0 30px;

          a{
            text-decoration: none;
            color: black;
            font-weight: 600;
            
          &:hover{
            color: blue;
          }
          }
        }
      }

        .button-wrapper{
          width: 200px;
          display: flex;
          align-items: center;
          justify-content: center;

          // button
          @import '../assets/button.scss';
        }
    }
  }
}

</style>
