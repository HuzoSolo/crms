<template>
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
</template>

<script>

import mainFlow from '/src/components/mainFlow.vue';
import sideBar from '/src/components/sideBar.vue';
import floatingButton from '/src/components/floatingButton.vue';

export default {
  data() {
    return {
      user: {
        name: this.$route.params.email,
        id: 1,
      },
    };
  },
 components: {
  mainFlow,
  sideBar,
  floatingButton,
 },
};

</script>

<style lang="scss">

</style>
