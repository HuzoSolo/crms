<template>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
    integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ=="
    crossorigin="anonymous"
    referrerpolicy="no-referrer"
  />
  <div class="" id="app">
    <div class="row">
      <!-- left side -->
      <div class="col-sm-1 col-m-1 col-lg-1 col-xl-1 rounded-3">
        <nav class="">
          <sideBar></sideBar>
        </nav>
      </div>

      <!--middle space-->
      <div class="col-sm-11 col-m-11 col-lg-11 col-xl-11">
        <mainFlow></mainFlow>
      </div>
    </div>
    <floatingButton></floatingButton>
  </div> 
  <router-view/>
</template>

<script> 
  export default {

  };
</script>

<style lang="scss">
@import "./assets/scss/index.scss";
</style>
