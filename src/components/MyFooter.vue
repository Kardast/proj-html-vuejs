<template>
  <div class="my-footer">

    <!-- Footer will contain logo and links on the middle and social on the bottom -->
    <div class="footer-top">

        <div class="f-wrapper">

            <div class="f-about">

                <h3>ABOUT</h3>

                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nobis quia vel iusto fuga ratione error ullam iure cumque a vitae libero delectus laboriosam, nisi assumenda. A libero eligendi exercitationem neque?</p>
                <img src="../assets/img/avada-movers-logo.png" alt="avada movers">
            </div>

            <div class="f-movers">

                <h3>AVADA MOVERS</h3>

                <ul>

                    <li 
                    v-for="(item, i) in footerLinks" 
                    :key="i"
                    @click="activeHere(item)"
                    >
                        <a :class="item.active === true ? 'here' : '' " href="#"><font-awesome-icon icon="fa-solid fa-angle-right" /> {{item.link}}</a>
                    </li>
                </ul>

            </div>

            <div class="f-posts">

                <h3>RECENT POSTS</h3>

                <ul>

                    <li 
                    v-for="(item, k) in footerPosts" 
                    :key="k"
                    >
                        <a href="#"><font-awesome-icon icon="fa-solid fa-angle-right" /> {{item.link}}</a>
                    </li>
                </ul>

            </div>
        </div>
    </div>

    <div class="footer-bottom">

        <div class="f-copyright">

            <p>
                &copy; Copyright 2012 - 2022 &vert; Avada Theme by ThemeFusion &vert; All Rights Reserved &vert; Powered by WordPress
            </p>
        </div>

        <!-- My Socials -->
        <ul class="f-socials">

            <li v-for="(item, j) in footerSocial" :key="j">
                <a href="#">
                <font-awesome-icon :icon="item.social" />
                </a>
            </li>
        </ul>

    </div>
  </div>
</template>

<script>


export default {
    name: 'MyFooter',

    props: {
        footerLinks: Array,
        footerPosts: Array,
        footerSocial: Array
    },

    methods: {
    // function that changes "here" class
    activeHere(myItem){
      this.footerLinks.forEach(element => {
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
.my-footer{
    width: 100%;
    background-color: #6abf17;
    height: 620px;
    padding-top: 20px;

    .footer-top{
        width: 100%;
        height: 480px;
        background-color: white;

        .f-wrapper{
            width: 70%;
            height: 100%;
            margin: 0 auto;
            display: flex;
            align-items: center;
            padding: 0 50px;

            li{

                list-style: none;
                margin: 40px 0;

                // here class
                @import '../assets/myGeneralCss.scss';

                a{

                    text-decoration: none;
                    color: black;

                    &:hover{
                        color: blue;
                    }
                }
            }

            .f-about{
                width: 300px;
                margin: 0 40px;
                min-width: 300px;

                p{
                    margin: 40px 0;
                    line-height: 30px;
                }
            }

            .f-movers{
                width: 300px;
                margin: 0 40px; 
                min-width: 300px;

            }

            .f-posts{
                width: 300px;
                margin: 0 40px;
                min-width: 300px;

            }
        }
    }

    .footer-bottom{
        width: 100%;
        height: calc(100% - 480px);

        .f-copyright{
            height: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
        }

        .f-socials{
            height: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            list-style: none;
            padding-bottom: 10px;

            li{
                margin: 0 15px;

                a{
                    color: white;
                }
            }

        }
    }
}

</style>
