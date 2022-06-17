<template>
  <div class="my-service-solution">

    <!-- This section will contain some text and 3 cards in the middle -->
    <div class="service-wrapper">

        <div class="service-text">

            <span>WE ARE A PROFESSIONAL</span>
            <h2>Full-Service Solution</h2>
        </div>

        <div class="cards-wrapper">

            <div class="service-card">

                <img src="" alt="">
                <h3>Two Man Teams</h3>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                <a class="button" href="#">READ MORE</a>
            </div>
            <div class="service-card">

                <img src="" alt="">
                <h3>Two Man Teams</h3>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                <a class="button" href="#">READ MORE</a>
            </div>
            <div class="service-card">

                <img src="" alt="">
                <h3>Two Man Teams</h3>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                <a class="button" href="#">READ MORE</a>
            </div>
        </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyServiceSolution',

}
</script>

<style lang="scss">
.my-service-solution{
    width: 100%;
    height: 620px;
    background-color: #ffffff;
    display: flex;
    align-items: center;

    .service-wrapper{
        width: 80%;
        height: 80%;
        margin: 0 auto;
        background-color: yellow;

        .service-text{
            text-align: center;
            background-color: blue;
            height: 80px;

            span{
                font-size: 13px;
                color: rgb(80, 80, 80);
                font-weight: 600;
            }

            h2{
                color: #6abf17;
                font-size: 30px;
            }

            p{
                width: 40%;
                margin: 0 auto;
                font-size: 14px;
                line-height: 25px;
                margin-bottom: 25px;
            }

        }

        .cards-wrapper{
            width: 70%;
            height: calc(100% - 80px);
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 0 auto;

            .service-card{
                background-color: red;
                width: 300px;
                height: 400px;
                // button
                @import '../assets/button.scss';
            }
        }
    }

}

</style>
