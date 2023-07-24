<template>
    <div class="container">
        <div class="row">
            <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                <div class="row">
                    <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                        <h3 class="text-center header m-3">Ders Ekle</h3>
                    </div>
                </div>
                <div class="row">
                    <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
                        <formsClassAdd></formsClassAdd>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import formsClassAdd from './formsClassAdd.vue';
export default {
    components: {
        formsClassAdd,
    },
    
}
</script>

<style lang="scss" scoped>

.header {
    color: #c13832;
}

</style>