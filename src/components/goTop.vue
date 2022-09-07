<template>
  <div class="goTop">
    <div>⌃</div>
    <div>TOP</div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    @import '../style/main.scss';

    .goTop {
        width: 50px;
        height: 50px;
        background-color:#40c4ff;
        position:absolute;
        bottom:0;
        right:0;
        text-align: center;
        color:white;
        font-size: 0.8em;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        
    }

</style>