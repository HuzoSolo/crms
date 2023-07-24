<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
        <div class="row">
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <h3 class="text-center header m-3">Ünite Ekle</h3>
          </div>
        </div>
        <div class="row">
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <formsSubjectAdd></formsSubjectAdd>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import formsSubjectAdd from './formsSubjectAdd.vue';    
export default {
    components: {
        formsSubjectAdd,
    },
    
};
</script>

<style>
.header {
    color: #c13832;
}
</style>