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
        <div class="col-sm-11 col-m-11 col-lg-11 col-xl-11">
            <saluteUser class="" id="#"></saluteUser>
            <!--Courses-->
            <adminCoursesSectionVue class="tab" id="courses"></adminCoursesSectionVue>
            <!--Sections-->
            <adminSectionsSectionVue class="tab" id="sections"></adminSectionsSectionVue>
            <!--Teachers-->
            <adminTeachersSectionVue class="tab" id="teachers"></adminTeachersSectionVue>
            <!--Students-->
            <adminStudentSectionVue class="tab" id="students"></adminStudentSectionVue>
            <!--Payments-->
            <adminPaymentsSectionVue class="tab" id="payments"></adminPaymentsSectionVue>
            <!--settings-->
        </div>
        </div>
    
  </div>
</template>

<script>
import saluteUser from '@/components/saluteUser.vue';
import adminSideBar from '@/components/adminSideBar.vue'
import adminCoursesSectionVue from '@/components/adminCoursesSection.vue'
import adminStudentSectionVue from '@/components/adminStudentSection.vue'
import adminTeachersSectionVue from '@/components/adminTeachersSection.vue'
import adminPaymentsSectionVue from '@/components/adminPaymentsSection.vue'
import adminSectionsSectionVue from '@/components/adminSectionsSection.vue'


export default {
    components: {
        saluteUser,
        adminSideBar,
        adminCoursesSectionVue,
        adminStudentSectionVue,
        adminTeachersSectionVue,
        adminPaymentsSectionVue,
        adminSectionsSectionVue,
        
    }
}
</script>

<style>

</style>