<template>
  <div class="shopLabel">
      <div class="circle">
          <img src="../assets/svg/svg-0.svg" alt="">
      </div>
      <div class="shop">
        <img src="../assets/svg/svg-1.svg" alt="">
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    .shopLabel {
        position: absolute;
        right:0;
        top:20;
        .circle , .shop {
            width: 25px;
            height: 25px;
            background-color: #F40A4A;
            margin-bottom: 10px;
            padding: 5px;

            img {
                width: 100%;
                object-fit: cover;
            }
        }
    }


</style>