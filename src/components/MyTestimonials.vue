<template>
  <div class="my-testimonials">

    <!-- This section will contain some text and 3 cards in the middle -->
    <div class="testimonials-wrapper">

        <div class="testimonials-text">

            <span>HAPPY CUSTUMERS</span>
            <h2>Testimonials</h2>
        </div>

        <div class="cards-wrapper">

            <div class="testimonials-card">

                <img src="../assets/img/avada-movers-johndoe-final-400x400.jpg" alt="john doe">
                <div class="texts">

                    <h3>John Doe</h3>
                    <p>"Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!"</p>
                </div>
            </div>
            <div class="testimonials-card">

                <img src="../assets/img/avada-movers-janedoe-final-400x400.jpg" alt="jane doe">
                <div class="texts">

                    <h3>Jane Doe</h3>
                    <p>"Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!"</p>
                </div>
            </div>
            <div class="testimonials-card">

                <img src="../assets/img/avada-movers-johnsmith-final-400x400.jpg" alt="john smith">
                <div class="texts">

                    <h3>John Smith</h3>
                    <p>"Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis, sequi, ipsum recusandae quasi rerum excepturi nulla porro incidunt blanditiis fugiat assumenda nesciunt beatae ipsa ducimus impedit accusantium veritatis, similique aspernatur!"</p>
                </div>
            </div>
        </div>

        <div class="button-wrapper">

            <a class="button" href="#">READ MORE TESTIMONIALS</a>
        </div>

    </div>
  </div>
</template>

<script>


export default {
  name: 'MyTestimonials',

}
</script>

<style lang="scss">
.my-testimonials{
    width: 100%;
    height: 800px;
    background-color: #ffffff;
    display: flex;
    align-items: center;
    background-image: url("../assets/img/avada-movers-testimonial-background.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    margin-bottom: 100px;


    .testimonials-wrapper{
        width: 80%;
        height: 80%;
        margin: 0 auto;
        padding-top: 30px;

        .testimonials-text{
            text-align: center;
            margin-bottom: 10px;

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
            height: calc(100% - 100px);
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 0 auto;

            .testimonials-card{
                width: 350px;
                height: 490px;
                padding: 15px;
                text-align: center;

                img{
                    width: 50%;
                    margin-bottom: 10px;
                    border-radius: 50%;
                }

                .texts{
                    padding: 20px 20px 25px 20px;
                    
                    h3{
                        color: #1775bf;
                        margin-bottom: 30px;
                    }
                    
                    p{
                        font-size: 14px;
                        line-height: 25px;
                        margin-bottom: 20px;
                        font-style: italic;
                    }
                }
            }
        }

        .button-wrapper{
            width: 300px;
            margin: 0 auto;
            text-align: center;

            // button
            @import '../assets/myGeneralCss.scss';
        }
    }
}

</style>
