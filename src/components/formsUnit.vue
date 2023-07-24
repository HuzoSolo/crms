<template>
    <div class="container">
        <div class="row">
            <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                <div class="row">
                    <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                        <h3 class="text-center header m-3">Konu Ekle</h3>
                    </div>
                </div>
                <div class="row">
                    <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                        <formsUnitAdd></formsUnitAdd>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
 import formsUnitAdd from './formsUnitAdd.vue';
export default {
   components: {
       formsUnitAdd,
   },

}
</script>

<style>

</style>