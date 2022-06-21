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

                <img src="../assets/img/avada-movers-serviceonephoto-final-400x255.jpg" alt="avada movers">
                <div class="texts">

                    <h3>Two Man Teams</h3>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                    <a class="button" href="#">READ MORE</a>
                </div>
            </div>
            <div class="service-card">

                <img src="../assets/img/avada-movers-servicetwophoto-final-400x255.jpg" alt="avada movers">
                <div class="texts">

                    <h3>We Do All The Lifting</h3>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                    <a class="button" href="#">READ MORE</a>
                </div>
            </div>
            <div class="service-card">

                <img src="../assets/img/avada-movers-servicethreephoto-final-400x255.jpg" alt="avada movers">
                <div class="texts">

                    <h3>Coast To Coast</h3>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!</p>
                    <a class="button" href="#">READ MORE</a>
                </div>
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
    height: 800px;
    background-color: #ffffff;
    display: flex;
    align-items: center;

    .service-wrapper{
        width: 80%;
        height: 80%;
        margin: 0 auto;

        .service-text{
            text-align: center;

            span{
                font-size: 13px;
                color: rgb(80, 80, 80);
                font-weight: 600;
            }

            h2{
                color: #6abf17;
                font-size: 30px;
                margin-top: 10px;
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
            min-width: 950px;
            height: calc(100% - 100px);
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 0 auto;

            .service-card{
                background-color: #f2f5f8;
                width: 300px;
                height: 490px;
                padding: 15px;
                text-align: center;

                img{
                    width: 100%;
                    margin-bottom: 10px;
                }

                .texts{
                    background-color: white;
                    padding: 20px 20px 25px 20px;
                    
                    h3{
                        color: #1775bf;
                        margin-bottom: 10PX;
                    }
                    
                    p{
                        font-size: 14px;
                        line-height: 20px;
                        margin-bottom: 20px;
                    }

                    // button
                    @import '../assets/myGeneralCss.scss';
                }

            }
        }
    }

}

</style>
