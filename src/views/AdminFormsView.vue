<template>
  <div class="" id="app">
    <div class="row">
      <!-- left side -->
      <div class="col-sm-1 col-m-1 col-lg-1 col-xl-1 rounded-3">
        <nav class="">
          <adminSideBar></adminSideBar>
        </nav>
      </div>

      <!--middle space-->
      <div class="col-sm-11 col-m-11 col-lg-11 col-xl-11 pb-5">
        <saluteUser class="" id="#"></saluteUser>
        <div class="row">
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <formsCategory class="p-4"></formsCategory>
          </div>
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <formsClass class="p-4"></formsClass>
          </div>
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <formsSubject class="p-4"></formsSubject>
          </div>
          <div class="col-sm-12 col-m-12 col-lg-12 col-xl-12">
            <formsUnit class="p-4"></formsUnit>
          </div>
        </div>
      </div>
    </div>
    <floatingButton @click="pushAdminForms"></floatingButton>
  </div>
</template>

<script>
import adminSideBar from "@/components/adminSideBar.vue";
import saluteUser from "@/components/saluteUser.vue";
import formsCategory from "@/components/formsCategory.vue";
import formsClass from "@/components/formsClass.vue";
import formsSubject from "@/components/formsSubject.vue";
import formsUnit from "@/components/formsUnit.vue";
import floatingButton from '/src/components/floatingButton.vue';

export default {
  components: {
    saluteUser,
    adminSideBar,
    formsCategory,
    formsClass,
    formsSubject,
    formsUnit,
    floatingButton,
  },
  methods: {
    //push the admin/forms route
    pushAdminForms() {
       this.$router.push("/admin");

     },
  },

};
</script>

<style>
.list-group-item {
  cursor: pointer;
}

</style>