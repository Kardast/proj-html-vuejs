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

          <li 
          v-for="(item, k) in headerLinks" 
          :key="k"
          @click="activeHere(item)"
          >
            <a :class="item.active === true ? 'here' : '' " href="#">
              {{item.link}}
            </a>
          </li>
        </ul>

          <div class="button-wrapper">

            <a class="button" href="#">FREE QUOTE</a>
        </div>
      </div>
    </div>

    <div class="scroll-up-box">
      <a href="#"><font-awesome-icon icon="fa-solid fa-angle-up" /></a>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyHeader',

  props: {
    headerSocial: Array,
    headerLinks: Array
  },

  methods: {
    // function that changes "here" class
    activeHere(myItem){
      this.headerLinks.forEach(element => {
        element.active = false
        if (element.active === false) {
          myItem.active = true
        } 
          console.log(1, element.active);
      });
    }
  }

}
</script>

<style lang="scss">
.my-header{
  width: 100%;
  height: 150px;
  background-color: rgba(255, 255, 255, 0.39);

  .scroll-up-box{
    width: 35px;
    height: 30px;
    background-color: #394132;
    position: fixed;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 3px;
    bottom: 0;
    right: 80px;

    a{
      color: white;
    }
  }
  
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
        min-width: 675px;
        display: flex;
        align-items: center;
        justify-content: end;
        list-style: none;

        li{
          margin: 0 30px;

        // here class
        @import '../assets/myGeneralCss.scss';

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
          @import '../assets/myGeneralCss.scss';
        }
    }
  }

}

</style>
