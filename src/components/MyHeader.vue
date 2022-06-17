<template>
  <div class="my-header">

    <!-- Header will be divided in two parts -->
    <div class="h-socials">

      <div class="htop-wrapper">

        <div class="telephone">

          <p> Call us for a Free Quote: 1.800.55.6789</p>
        </div>

        <ul class="socials">

          <li><a href="#">twitter</a></li>
        </ul>
      </div>
    </div>

    <div class="h-links">

      <div class="hbottom-wrapper">

      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'MyHeader'

}
</script>

<style lang="scss">
.my-header{
  width: 100%;
  height: 150px;
  // debug
  background-color: yellow;

  .h-socials{
    width: 100%;
    height: 50px;
    // debug
    background-color: #6abf17;

    .htop-wrapper{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      // debug
      background-color: blue;

      .telephone{
        width: 50%;
        display: flex;
        align-items: center;
      }

      .socials{
        width: 50%;
        display: flex;
        list-style: none;
      }
    }
  }

  .h-links{
    width: 100%;
    height: 100px;
    // debug
    background-color: #5f7e41;

    .hbottom-wrapper{
      width: 80%;
      height: 100%;
      margin: 0 auto;
      // debug
      background-color: rgb(55, 55, 139);
    }
  }
}

</style>
